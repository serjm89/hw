               How to use
## If u from the RU network segment use a proxy
## Information  https://home.treasury.gov/policy-issues/financial-sanctions/sanctions-programs-and-country-information 

## If u use ubuntu2204 - install latest gem net-ssh 
## https://rubygems.org/gems/net-ssh/versions

## Use proxy because prometheus-node-exporter dont install in RU segment 


git clone https://github.com/serjm89/hw

cd hw/ && vagrant up --provision

dashboard grafana: 
http://localhost:3000/d/rYdddlPWk/

username: admin
password: grafana
