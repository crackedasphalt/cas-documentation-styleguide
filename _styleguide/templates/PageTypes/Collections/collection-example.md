---
title: Collection-Example # Collection Name
layout: collection
permalink: /collection-example/
collection: collection-example
entries_layout: grid
classes: wide
---

## To create a collection for collection `collection-example`
1. Add or update _config.yml to include 
   ```markdown
   collections:
      collection-example:
        output: true
        permalink: /:collection/:path/
    ```
2. Create directory `_collection-example` at root
3. Copy this page to `/_pages`
4. Adjust in this page yaml front matter
   ```markdown
   title: # Give the page a title
   permalink: # Give this page a permalink 
   collection: # Populate with the name of the collection you defined in _config.yml
   ```
5. Optionally adjust other front matter to meet requirements.
6. Delete the content of this page outside of yaml front matter.