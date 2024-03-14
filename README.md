# Deployment

npm install --save-dev @types/debug@^4.1.7 @types/jest@^29.5.0 @types/node@^18.16.3 @types/node-rsa@^1.1.1 @types/sqlstring@^2.3.0 @types/supertest@^2.0.12 @typescript-eslint/eslint-plugin@^5.59.1 @typescript-eslint/parser@^5.59.1 eslint@^8.39.0 eslint-config-prettier@^8.8.0 eslint-plugin-prettier@^4.2.1 find-free-ports@^3.1.1 husky@^8.0.3 jest@^29.5.0 nock@^13.3.0 nodemon@^2.0.22 prettier@2.8.8 supertest@^6.3.3 testcontainers@^9.6.0 ts-jest@^29.1.0 ts-mockito@^2.6.1 ts-node@^10.9.1 typescript@^5.0.4


npm install class-transformer@^0.5.1 debug@^4.3.4 dotenv@^16.4.5 fast-xml-parser@^4.2.2 find-my-way@^7.6.0 hyper-express@^6.5.9 kafkajs@^2.2.4 mariadb@^3.1.2 node-rsa@^1.1.1 redis@^4.6.6 reflect-metadata@^0.1.13 sqlstring@^2.3.3 toad-scheduler@^2.2.0 winston@^3.8.2


curl  -X POST \
  'localhost:3000/token/api/ReqUpdateToken/2.0/urn:txnid:NPCI1234567890' \
  --header 'Accept: */*' \
  --header 'User-Agent: Thunder Client (https://www.thunderclient.com)' \
  --header 'Content-Type: application/xml' \
  --data-raw '<ns2:ReqUpdateToken xmlns:ns2="http://npci.org/token/schema/">
<Head ver="2.0" ts="" orgId="129751" msgId=""/>
<ReqDetails type="CHECKREDEEM">
<Details>
<Detail name="requestId" value="123456"/>
</Details>
<Amount value="12.00" curr="INR">
<Denominations>
<Denomination value="10.00" count="1"/>
<Denomination value="2.00" count="1"/>
</Denominations>
</Amount>
</ReqDetails>
</ns2:ReqUpdateToken>'
