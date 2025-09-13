
## Installation

Download and install NodeJs https://nodejs.org/en/download

#### Check nodeJS and npm versions:

node -v
npm -v

#### Initialize the project

cd <project_path>
npm init -y

#### Install core test stack

npm install -D playwright @playwright/test typescript ts-node
npx playwright install
npm install uuid

#### Install extras

npm install -D @faker-js/faker dotenv

#### Install your preferred mock server

npm install -D json-server

#### Install custom routes

npm install -D express

#### Install Express

npm install -D express body-parser
npm install --save-dev @types/express @types/node
npm install --save-dev ts-node typescript

#### Install TSX

npm install -D tsx

## UI Set up

Step 1: Set up React Project (Vite)
npm create vite@latest frontend -- --template react-ts
cd frontend
npm install

## Run localhost Dev Server

`npx ts-node mocks/server.ts`

## Run Tests

**UI Tests** (Run from root of the project):

Run dev server before running UI tests

`npx ts-node mocks/server.ts`

Run Tests

`npx playwright test tests/ui/user_ui.spec.ts`

`npx playwright test tests/ui/transaction_ui.spec.ts`

**API Tests:** 

Run from root of the project:

`npx playwright test tests/api --headed`

**Localhost URL**

http://localhost:3000

http://localhost:3000/user_crud.html

http://localhost:3000/transactions_crud.html
