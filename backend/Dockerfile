FROM node:22

WORKDIR /backend-app
COPY package.json ./
RUN npm install
COPY index.js ./
COPY .env ./





















EXPOSE 5050

CMD [ "npm", "start" ]


# 1. Navigate to the `backend` directory:

#     ```sh
#     cd backend
#     ```
 
#  2. Install the required dependencies:
 
#     ```sh
#     npm install
#     ```
 
#  3. Create a `.env` file in the `backend` directory with the following content:
 
#     ```
#     DATABASE_URL=postgres://postgres:password@localhost:5432/mydatabase
#     ```
 
#     Make sure to replace `password` with your actual PostgreSQL password.
 
#  4. Start the back-end server:
 
#     ```sh
#     npm start
#     ```
 
#     The back-end server should now be running at `http://localhost:5050`.