# Name Profiling API
## Overview
This is a RESTful API built with Node.js+Express for managing meta information on names. It provides `GET`, `POST`, and `DELETE` operations with proper error handling.

## Project Structure
```
stage_1
├── package.json
├── package-lock.json
├── README.md
├── src
│   ├── controllers
│   │   └── profileController.ts
│   ├── db
│   │   └── conn.ts
│   ├── model
│   │   └── nameMeta.ts
│   ├── routes
│   │   └── profileRoute.ts
│   └── server.ts
└── tsconfig.json
```

## Technologies Used
- Node.js
- Express
- Typescipt

## Installation
NOTE: You should have `git` and `node` installed already
1. clone the repository
```bash
git clone git@github.com:Amaryllis750/hng14-stage1-profileapi.git
cd hng14-stage1-profileapi
```

2. Install dependencies
```bash 
npm install 
```

## Running the server
To run the server in development mode
``` bash
npm run dev
```

NOTE: You can start the server in production mode using
```bash
npm run start
```
But you must build the project first with `npm run build`


## API Endpoints
- `POST /api/profiles` - Create a new profile for a name
- `GET /api/profiles/:id` - Get a particular profile by the id
- `GET /api/profiles` - Get all profiles available
- `DELETE /api/profiles/:id` - Delete profile by Id

## Profile Schema
```json
{
      "id": "019d98fa-3f2c-7316-acc9-338738a1faa2",
      "name": "daniel",
      "gender": "male",
      "gender_probability": null,
      "sample_size": 2466344,
      "age": 58,
      "age_group": "adult",
      "country_id": "ro",
      "country_probability": null,
      "created_at": "2026-04-17T01:07:10.247Z"
    }
```

## Support
For support, open an issue.