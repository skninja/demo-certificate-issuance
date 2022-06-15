## ref-sunbirdrc-certificate
Reference sample of certificate registry using Sunbird RC

# Run your own certificate registry in 5 minutes 


Prerequesite:

* docker
* docker-compose
* git (or download the zip)

1. run `git clone https://github.com/dileepbapat/ref-sunbirdrc-certificate.git`
2. cd ref-sunbirdrc-certificate
3. run `docker-compose pull`
4. run `docker-compose up -d --force-recreate`

API sample is available in jupyter notebook, needs additional dependency of python and jupyter. 
check certificate-api.ipynb

## Troubleshooting
run `docker-compose logs -f registry` and check logs


# Frontend - certificate registry setup

Prerequesite:
* Angular 10.2.1
* nodejs and npm

1. Clone Sunbird RC UI code from here - <https://github.com/code-blooded-guy/sunbird-rc-ui/tree/issuance>
2. Clone **UI config files** from git - <https://github.com/Sunbird-RC/demo-certificate-issuance>
3. Go to into the ***demo-education-registry/ui-config*** and **copy this folder path**
4. Then go to into the **/sunbird-rc-ui/src/assets/config folder**  and open terminal 

Run blow command in the following folder path : ***sunbird-rc-ui/src/assets/config***

|ln -s (***path-of-your-UI-config files folder***)|
| :- |

Eg : **ln -s *demo-education-registry/ui-config*** 


5. Add your **config.json** and **home.html** file on below mentioned path
***sunbird-rc-ui/src/assets/config***

6. Go to root folder means **sunbird-rc-ui** folder 
Run - **npm start**

7. Once project run completely then you will get <http://localhost:4200> url
to open an angular application in the browser.

8. Copy that url( <http://localhost:4200>) and paste in your browser.

- Reference document : <https://docs.sunbirdrc.dev/use/setup-the-frontend>

