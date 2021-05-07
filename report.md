# Отчёт о тестировании приложения Credit Card Number Validator

## Краткое описание

07.05.2021 было проведено тестирование приложения Credit Card Number Validator положительными и отрицательными данными.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты: [Issue #1](https://github.com/goso-nct/netology-java-dz1.1-t1/issues/1)

## Описание процесса тестирования

В файле Main.java изменялось значение поля number и запускалась программа.

В качестве тестовых использовались данные с сайта:  
https://www.freeformatter.com/credit-card-number-generator-validator.html.

### Положительное тестирование:

* VISA:  
4716997104136332 Ex.R: OK, Act.R: OK  
4485647592840338 Ex.R: OK, Act.R: OK  
4929463495548897535 Ex.R: **OK**, Act.R: **FAIL**


* MasterCard:  
2221001644042548 Ex.R: OK, Act.R: OK  
5354560066891486 Ex.R: OK, Act.R: OK  
2720992231021844 Ex.R: OK, Act.R: OK  


* American Express (AMEX):  
370378424982769 Ex.R: **OK**, Act.R: **FAIL**  
377272667344741 Ex.R: **OK**, Act.R: **FAIL**  
342211276519915 Ex.R: **OK**, Act.R: **FAIL**  


* Discover:  
6011345587017172 Ex.R: OK, Act.R: OK  
6011226607108995 Ex.R: OK, Act.R: OK  
6011557939298835700 Ex.R: **OK**, Act.R: **FAIL**  


* JCB:  
3589917309008025 Ex.R: OK, Act.R: OK  
3535713953227598 Ex.R: OK, Act.R: OK  
3541606355638606828 Ex.R: **OK**, Act.R: **FAIL**  


* Diners Club - North America:  
5489428177558279 Ex.R: OK, Act.R: OK  
5405060275666026 Ex.R: OK, Act.R: OK  
5461698193272905 Ex.R: OK, Act.R: OK  


* Diners Club - Carte Blanche:  
30068368702685 Ex.R: **OK**, Act.R: **FAIL**  
30577886809764 Ex.R: **OK**, Act.R: **FAIL**  
30142479795290 Ex.R: **OK**, Act.R: **FAIL**  


* Diners Club - International:  
36880739212168 Ex.R: **OK**, Act.R: **FAIL**  
36023097189369 Ex.R: **OK**, Act.R: **FAIL**  
36527645219015 Ex.R: **OK**, Act.R: **FAIL**  


* Maestro:  
6761976956950890 Ex.R: OK, Act.R: OK  
6762412751670920 Ex.R: OK, Act.R: OK  
5893853803565457 Ex.R: OK, Act.R: OK  


* Visa Electron:  
4844801128131847 Ex.R: OK, Act.R: OK  
4175003981595379 Ex.R: OK, Act.R: OK  
4026883892918591 Ex.R: OK, Act.R: OK  


* InstaPayment:  
6394460600222530 Ex.R: OK, Act.R: OK  
6397623636981620 Ex.R: OK, Act.R: OK  
6396533955116313 Ex.R: OK, Act.R: OK  

### Отрицательное тестирование:

пустая строка  Ex.R: FAIL, Act.R: FAIL  
abc  Ex.R: FAIL, Act.R: FAIL  
6011345587017171 Ex.R: FAIL, Act.R: FAIL  
5550477361880754 Ex.R: FAIL, Act.R: FAIL  
348272279557558 Ex.R: FAIL, Act.R: FAIL  

## Тестирование производилось в следующем окружении:
* Windows 10 Pro 20H2 64bit
* AdoptOpenJDK-11.0.11+9 64bit HotSpot
* IntelliJ IDEA 2021.1.1 Build #IU-211.7142.45

