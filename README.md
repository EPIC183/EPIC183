- š Hi, Iām @EPIC183
- š Iām interested in 
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
EPIC183/EPIC183 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
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
