## Free Fire Item Data

A comprehensive JSON dataset containing item information for Garena Free Fire, providing developers and enthusiasts with structured game data for various applications.

## 📁 Data Source

The item data is available at:

```
https://raw.githubusercontent.com/I-SHOW-AKIRU/item/main/ItemData.json
```

Access the JSON data directly using the raw GitHub URL:

**javascript Example**
```javascript
const itemDataUrl = 'https://raw.githubusercontent.com/I-SHOW-AKIRU/item/main/ItemData.json';

// Fetch example in JavaScript
fetch(itemDataUrl)
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error loading data:', error));
```

**Python Example**

```python
import requests
import json

url = "https://raw.githubusercontent.com/I-SHOW-AKIRU/item/main/ItemData.json"
response = requests.get(url)
item_data = response.json()

print(f"Loaded {len(item_data)} items")
```

## Data Structure

The JSON file contains an array of Free Fire items with the following structure:

**Example Item Object**

```json
[
    {
        "Id": 101000001,
        "Type": "AVATAR",
        "collectionType": "NONE",
        "name": "Nulla",
        "desc": "Nobody knows how she got onto Bermuda, except that she was here before everyone else. Extremely good at adapting to the environment, she is like a chameleon that survives and thrives.",
        "Icon": "Icon_face_female01_head",
        "Rare": "NONE",
        "IsUnique": true,
        "IconInAB": "Icon_In_CDN"
    }
]
```

**Field Descriptions**

- **Id**: Unique numeric identifier for the item
- **Type**: Category of the item (e.g., AVATAR, WEAPON, etc.)
- **collectionType**: Collection classification
- **name**: Display name of the item (may be null for some entries)
- **desc**: Detailed description of the item (may be null for some entries)
- **Icon**: Reference to the item's icon asset
- **Rare**: Rarity classification of the item
- **IsUnique**: Boolean indicating if the item is unique
- **IconInAB**: Asset bundle reference for the icon

## Use Cases

**This dataset can be used for:**

- **Game Development**: Building companion apps or tools for Free Fire
- **Fan Sites**: Creating item databases and wikis
- **Educational Projects**: Learning JSON data handling and API integration
- **Bot Development**: Creating Discord bots, Telegram bots or other automated systems
- **Mobile Applications**: Building Free Fire utility apps

## Notes

- Data is maintained by the community and requires periodic updates
- Some entries may have null values for name and desc fields
- This is an unofficial resource not affiliated with Garena Free Fire
- Always respect the game's terms of service when using this data
- Consider caching the data to avoid frequent API calls

## Data Quality

- The dataset includes items with complete and partial information
- Some entries serve as placeholders with null values
- Recommended to filter items with valid names for user-facing applications

## 🤝 Contributing

**Contributions to improve the dataset are welcome. Please ensure:**

- Data accuracy and consistency
- Proper formatting according to existing structure
- Clear commit messages describing changes
- Validation of new entries against the existing schema

## 📄 License

This project is provided for educational and development purposes. Please check the repository for specific licensing information.
