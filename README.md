# Defining HLC Healthcare's Marketing Strategy with AB Testing

Hello there! We are going to try to define best marketing strategy of HLC Healthcare with AB Testing. First of all lets talk about what is AB Testing and what is used for?

## What is AB Test
AB testing also known as Independent Samples T Test is a way of demonstrating whether there is statistical difference between two variables or not. For instance which marketing team performs more sales performance than other or which add to cart button our customers prefer most etc. We have two assumptions for AB Test. First of them is Normality other one is Equal Variances. If are assumptions are correct, we are going to apply Parametric tests, and Non-Parametric if they are not.

## Problem
HLC Healthcare sends e-mail and push notifications to its customers in different time to make sale and wants to know which method is better. Should HLC Healthcare sends e-mail or push notification in order to achive more successful marketing strategy. Both strategies cost equally and use same service provider.

## Application of AB Test
First we need to import needed libraries and data which has information of total_emails_send, total_notification_send, comebacks, customers_bought, profit
```python
df_email = pd.read_excel('../input/hlc-healthcare/hlc_healthcare.xlsx',sheet_name='Email Grubu',usecols=['mail_sayisi','geridonus','satin_alan_kisi','kazanc'])

df_push = pd.read_excel('../input/hlc-healthcare/hlc_healthcare.xlsx',sheet_name='Push Notification Grubu',usecols=['bildirim_sayisi','geridonus','satin_alan_kisi','kazanc'])
```
* mail_sayisi = total_emails_send
* geridonus = comeback
* satin_alan_kisi = customers_bought
* kazanc = profit
* bildirim_sayisi = total_notification_send

See more in code page.
