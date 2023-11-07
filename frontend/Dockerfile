From node:16.14.2 as build

#Building the frontend
WORKDIR /app

COPY . .
Run npm i

Run npm run build

FROM nginx:latest

COPY --from=build /app/build /etc/nginx/html
