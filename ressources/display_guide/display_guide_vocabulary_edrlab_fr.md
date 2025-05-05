---
layout: document
date: 2025-05-05
title: "Recommandations pour l'affichage des informations d'accessibilité"
previous: ../pages/diffuser.html
titlePrev: Informer
draft: false
---

 <section hidden="hidden">
 <select id="json-source-select">
 <option value="https://w3c.github.io/publ-a11y-display-guide-localizations/lang/fr-FR/display_guide_vocabulary_edrlab.json">EDRLab fr-FR</option>
 </select>
 </section>
 <section id="tables-container"></section>

 <script>
 // Function to fetch JSON data
async function fetchJsonData(url) {
 try {
 const response = await fetch(url);
 if (!response.ok) {
 throw new Error(`HTTP error status: ${response.status}`);
 }
 return await response.json();
 } catch (error) {
 console.error('Error fetching JSON:', error);
 }
}

// Function to create lists and tables for each key-value pair
function createListsAndTables(data, parentContainer) {
 // Set the lang attribute based on the language key
 const language = data.metadata.language;
 parentContainer.setAttribute('lang', language);
 Object.keys(data).forEach(key => {
 if (key === 'metadata') {
 const metadataList = document.createElement('ul');
 Object.keys(data[key]).forEach(subKey => {
 const listItem = document.createElement('li');
 const spanKey = document.createElement('span');
 spanKey.className = 'inline-list-item';

 spanKey.textContent = subKey;
 const spanValue = document.createElement('span');
 spanValue.textContent = data[key][subKey];
 listItem.appendChild(spanKey);
 listItem.appendChild(document.createTextNode(': ')); 
 listItem.appendChild(spanValue);
 metadataList.appendChild(listItem);
 });
 parentContainer.appendChild(document.createElement('h2')).textContent = 'Informations concernant ce vocabulaire';
 parentContainer.appendChild(metadataList);
 } else if (typeof data[key] === 'object') {
 // Find the title key within the object
 const titleKey = Object.keys(data[key]).find(subKey => subKey.endsWith('-title'));
 const titleValue = titleKey ? data[key][titleKey] : key;

 // Display the title
 const tableHeading = document.createElement('h2');
 tableHeading.innerHTML = `<span class="key">${key}</span>: <span class="value">${titleValue}</span>`;
 parentContainer.appendChild(tableHeading);

 // Check if there are any descriptive keys
 const descriptiveKeys = Object.keys(data[key]).filter(subKey => typeof data[key][subKey] === 'object' && data[key][subKey].descriptive);

 if (descriptiveKeys.length > 0) {
 // Create table if descriptive keys are present
 const table = document.createElement('table');
 const tableHeader = document.createElement('thead');
 const tableBody = document.createElement('tbody');

 // Create table header
 const headerRow = document.createElement('tr');
 headerRow.innerHTML = `
    <th>Key ID</th>
    <th>Descriptive sentence</th>
    <th>Compact sentence</th>
 `;
 tableHeader.appendChild(headerRow);

 // Create table body
 descriptiveKeys.forEach(subKey => {
    const row = document.createElement('tr');
    row.innerHTML = `
    <td>${subKey}</td>
    <td>${data[key][subKey].descriptive}</td>
    <td>${data[key][subKey].compact}</td>
    `;
    tableBody.appendChild(row);
 });

 // Assemble the table
 table.appendChild(tableHeader);
 table.appendChild(tableBody);

 parentContainer.appendChild(table);
 } else {
 // If no descriptive keys are present, display a list of all subkeys
 const subkeysList = document.createElement('ul');
 Object.keys(data[key]).forEach(subKey => {
    if (subKey !== titleKey) { // Exclude the title key if it exists
    const listItem = document.createElement('li');
    const keySpan = document.createElement('span');
    keySpan.className = 'key';
    keySpan.textContent = subKey;
    const valueSpan = document.createElement('span');
    valueSpan.className = 'value';
    valueSpan.textContent = data[key][subKey];
    listItem.innerHTML = `<span class="key">${subKey}</span>: <span class="value">${data[key][subKey]}</span>`;
    subkeysList.appendChild(listItem);
    }
 });
 parentContainer.appendChild(subkeysList);
 }

 // Handle subsets of additional-accessibility-information
 if (key === 'additional-accessibility-information') {
 Object.keys(data[key]).forEach(subSubsetKey => {
    if (typeof data[key][subSubsetKey] === 'object' && subSubsetKey.endsWith('-title')) {
    const subsetTitle = data[key][subSubsetKey];
    const subsetHeading = document.createElement('h3');
    subsetHeading.textContent = subsetTitle;
    parentContainer.appendChild(subsetHeading);

    const subsetDescriptiveKeys = Object.keys(data[key]).filter(subKey => subKey.startsWith(subSubsetKey.replace('-title', '')) && typeof data[key][subKey] === 'object' && data[key][subKey].descriptive);
    if (subsetDescriptiveKeys.length > 0) {
    const subsetTable = document.createElement('table');
    const subsetTableHeader = document.createElement('thead');
    const subsetTableBody = document.createElement('tbody');

    // Create table header
    const subsetHeaderRow = document.createElement('tr');
    subsetHeaderRow.innerHTML = `
    <th>Key ID</th>
    <th>Descriptive sentence</th>
    <th>Compact sentence</th>
    `;
    subsetTableHeader.appendChild(subsetHeaderRow);

    // Create table body
    subsetDescriptiveKeys.forEach(subKey => {
    const row = document.createElement('tr');
    row.innerHTML = `
     <td>${subKey}</td>
     <td>${data[key][subKey].descriptive}</td>
     <td>${data[key][subKey].compact}</td>
    `;
    subsetTableBody.appendChild(row);
    });

    // Assemble the table
    subsetTable.appendChild(subsetTableHeader);
    subsetTable.appendChild(subsetTableBody);

    parentContainer.appendChild(subsetTable);
    } else {
    // If no descriptive keys are present in the subset, display a list of all subkeys
    const subsetSubkeysList = document.createElement('ul');
    Object.keys(data[key]).forEach(subKey => {
    if (subKey.startsWith(subSubsetKey.replace('-title', '')) && subKey !== subSubsetKey) {
     const listItem = document.createElement('li');
     const keySpan = document.createElement('span');
     keySpan.className = 'key';
     keySpan.textContent = subKey;
     const valueSpan = document.createElement('span');
     valueSpan.className = 'value';
     valueSpan.textContent = data[key][subKey];
     listItem.innerHTML = `<span class="key">${subKey}</span>: <span class="value">${data[key][subKey]}</span>`;
     subsetSubkeysList.appendChild(listItem);
    }
    });
    parentContainer.appendChild(subsetSubkeysList);
    }
    }
 });
 }
 }
 });
}

// Function to initialize the list and table creation
function initializeListAndTableCreation(data) {
 const tablesContainer = document.getElementById('tables-container');
 tablesContainer.innerHTML = ''; // Clear the container before populating it

 createListsAndTables(data, tablesContainer);
}

// Event listener for select change
document.getElementById('json-source-select').addEventListener('change', async function() {
 const selectedUrl = this.value;
 fetchJsonData(selectedUrl)
 .then(data => initializeListAndTableCreation(data))
 .catch(error => console.error('Error creating lists and tables:', error));
});

// Load initial JSON data and create lists and tables
const initialUrl = document.getElementById('json-source-select').value;
fetchJsonData(initialUrl)
 .then(data => initializeListAndTableCreation(data))
 .catch(error => console.error('Error creating lists and tables:', error));
 </script>

