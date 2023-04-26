FROM ${{values.node_js_version}}
WORKDIR /app
COPY package*.json .
COPY yarn.lock .
RUN npm install
COPY . ./
RUN npm run build
CMD "node dist/src/main.js"
