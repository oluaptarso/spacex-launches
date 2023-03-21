# SpaceX - Launches

SpaceX - Launches is an application that relies on the unofficial [SpaceX-API](https://github.com/r-spacex/SpaceX-API) to show SpaceX launches information.
<br />

The web application has four core functionalities:
- Fetch and display the next launch from the API and show it in a card;
- Fetch and display the previous launch from the API and show it in a card;
- Fetch and display the incoming launches from the API and show them on a list with infinite scroller;
- Fetch and display the past launches from the API and show them on a list with infinite scroller;

The API has 5 endpoints:
- /spacex-api/launches/latest : Returns the latest launch
- /spacex-api/launches/next : Returns the next launch
- /spacex-api/launches/upcoming : Return the upcoming launches
- /spacex-api/launches/past : Return the past launches
- /spacex-api/launches/next_and_latest : Returns the next and the latest launches

You can check the working version [here](https://spacexlaunches.paulotarso.dev).

## Meta repository

This meta[¹](#meta) repository manages the multi-project web application.

## Projects

### **[spacex-launches-api](https://github.com/oluaptarso/spacex-launches-api)**:
Backend REST API project, developed with [Nest](https://nestjs.com)

### **[spacex-launches-web-app](https://github.com/oluaptarso/spacex-launches-web-app)**:
Frontend web application project, developed with [Next.js](https://nextjs.org)

## Requirements
- Node.js - ^14.20.0 || ^16.13.0 || >=18.10.0 (The project was developed using 16.17.1);
- npm - 8.19.2+.

Visual Studio Code is optional but is highly recommended.

## How to install
Install meta using npm or yarn:

```bash
npm i -g meta
# or
yarn global add meta
```

Clone the meta and children repositories using git meta:

```
meta git clone https://github.com/oluaptarso/spacex-launches
```

Install the meta project dev dependencies:
```
cd spacex-launches
```
```bash
npm install
# or
yarn
```

Install the dependencies of the projects:
```bash
meta-npm install
# or
meta-yarn install
```

## How to run using docker
```bash
docker compose up
```
Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Running/Debugging using Visual Studio Code

There are four launch configurations to debug in VS Code, one for the API:
- API (NestJs): Debug server

And three options for the web application:
- WebApp (Next.js): Debug server-side;
- WebApp (Next.js): Debug client-side;
- WebApp (Next.js): Debug full stack.



## Additional information

<a name="meta"></a>¹ - [meta](https://github.com/mateodelnorte/meta#readme) is a tool for managing multi-project systems and libraries.
