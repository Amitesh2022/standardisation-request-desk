# Standardisation Request Desk

## One-sentence benefit
Helps policy teams, standards bodies and industry coordinate technical evidence and consensus-ready standardisation requests.

## Live demo
Run the Java service and Vue application locally to use the complete experience.

## Screenshots
![standardisation request workspace](docs/screenshot.png)

## Main features
Search standardisation requests, add a realistic pilot, progress evidence, inspect priorities and open dedicated standardisation guidance.

## Technology used
Vue, TypeScript, Pinia, Vue Router, Vite, Spring Boot and Java.

## Installation instructions
Start the backend with `cd backend && mvn spring-boot:run`. In another terminal run `npm install && npm run dev`.

## Commercial licensing/contact
Commercial licensing and implementation support are available through the repository owner.

## Business problem and users
Policy teams, standards bodies, industry experts and civil-society participants need a shared view of technical evidence, consultation readiness and accountable owners.

## Key workflows
Users can filter standardisation requests, create a Brussels standardisation case, move a project forward and open dedicated standardisation guidance.

## Vue framework highlights
The application uses the Composition API, Pinia computed state, reactive filters and Vue Router pages.

## Java backend highlights
The Spring Boot service provides real list, search, create and update endpoints, validation, clear errors, health reporting and tests.

## Architecture and state flow
Pinia owns the shared client state and synchronises it with the Java API after reads and writes.

## Accessibility and responsive behaviour
Landmarks, labels, visible focus, readable status text and responsive panels support keyboard and mobile users.

## Verification commands
Use `npm test`, `npm run build`, and `cd backend && mvn test package`.

## Structure
`src` contains the Vue experience, `backend` contains the Java service, and `docs` contains verified media.

## Tradeoffs
The demonstration uses an in-memory data store; production deployment would add authentication, persistence, standards catalogue links and standardisation-model integrations.

## Roadmap
Add standards catalogue imports, reference standards, standardisation scenarios, stakeholder consultation rooms and durable storage.
