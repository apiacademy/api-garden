# Architectural Components

## Backend Core
All the API styles should use the same core backend that will itself provide an API to use.  When implementing an API style, the backend will be built on top of this core.  The core contains the internal, implementation, including data storage and simulated functions.  It should only be accessed by the API layer - never from the frontend directly.

### Constraints
1.  Avoid Data Persistence - to keep the system lightwight and simple, data should be stored in memory only.
1.  Only for use by the "API Layer"
1.  No breaking changes allowed
1.  The Backend Core can be accessed via network based APIs (there will probably be more than one for each part of the system)

## API Backend
Exposes the API and handles messages.  This is the primary component that needs to built for each API style.  It can be written in any language.

## Web Frontend
A browser based front end client for the API.  WIth the exception of a few pages, the content and UX should be consistent for all API styles.  

# Web Content

## 
