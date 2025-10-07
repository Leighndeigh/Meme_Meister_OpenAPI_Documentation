## Overview

The **Meme Meister API** by **MemeMeister** allows developers to generate, manage, and retrieve memes programmatically.  
It takes an image and text captions, combines them, and returns a new meme image.

### Features
- **Create** memes with custom captions  
- **List** all existing memes  
- **Retrieve** a meme by ID  
- **Delete** memes from your collection  

All endpoints return **HTTP 200** upon success and consume/produce **JSON** unless otherwise specified.

---

## Security

Authentication uses **Facebook OAuth 2.0** with an **implicit flow**.  
Users authenticate via Facebook to gain access to meme creation and retrieval features.

### OAuth Configuration

| Property | Value |
|-----------|--------|
| **Type** | oauth2 |
| **Flow** | implicit |
| **Authorization URL** | `https://dev.facebook.com/oauth/authenticate` |
| **Description** | Facebook authentication for Meme Meister |
| **Scopes** | `write:memes` → Modify memes in your account <br> `read:memes` → Read memes in your account |
