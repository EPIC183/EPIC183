- 👋 Hi, I’m @EPIC183
- 👀 I’m interested in 
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
EPIC183/EPIC183 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
{
  "$id": "https://github.com/DeadlyKitten/MonkeModInfo/mods.schema.json",
  "type": "object",
  "required": ["mods", "groups"],
  "properties": {
    "mods": {
      "type": "array",
      "items": { "$ref": "#/$defs/mod" }
    },
    "groups": {
      "type": "array",
      "items": { "$ref": "#/$defs/group" }
    }
  },
  "$defs": {
    "mod": {
      "type": "object",
      "required": ["name", "gitPath", "releaseId", "author", "group"],
      "properties": {
        "name": {
          "type": "string"
        },
        "tag": {
          "type": "string"
        },
        "gitPath": {
          "type": "string"
        },
        "releaseId": {
          "type": "integer"
        },
        "author": {
          "type": "string"
        },
        "group": {
          "type": "string"
        }
      }
    },
    "group": {
      "type": "object",
      "required": ["name", "rank"],
      "properties": {
        "name": {
          "type": "string"
        },
        "rankd": {
          "type": "integer"
        }
      }
    }
  }
}
