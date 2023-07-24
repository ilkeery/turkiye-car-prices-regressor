# Turkiye Car Prices estimator (2020 data)

> Important: on branch ilker, i tried to handle the data as TIME SERIES and i tried new preprogres methods i believe useful.
## 1. Problem Definition
In our case, the problem we will be exploring is **regression** (predict dependent variable thanks to independent variables). 

This is because we're going to be using a number of different **features** (pieces of information) about a car to predict it's sale price

In a statement,

> Given features about a car, can we predict sale price?

## 2. Data

The original data came from the (https://www.kaggle.com/datasets/alpertemel/turkey-car-market-2020).


Attributes and features are also referred to as **independent variables** and a target variable can be referred to as a **dependent variable**.

> We use the independent variables to predict our dependent variable.


### Car Market in Turkiye Data Dictionary

A data dictionary describes the data you're dealing with. Not all datasets come with them so this is where you may have to do your research or ask a **subject matter expert** (someone who knows about the data) for more.

The following are the features we'll use to predict our target variable (heart disease or no heart disease).

The variables in the data set are as follows:

1. İlan Tarihi: Date
2. Marka: Brand
3. Arac Tip Grubu: Vehicle Type Group
4. Arac Tip: Vehicle Type
5. Model Yıl: Model Year
6. Yakıt Turu: Fuel Type (Benzin: Petrol, Dizel: Diesel, Benzin / LPG: Gasoline, Hibrit: Hybrid, Elektrik: Electricity)

7. Vites: Transmission (Otomatik: Automatic, Yarı Otomatik: Semi Automatic, Düz: Manual)
8. CCM: CCM
9. Beygir Gucu: Horse Power
10. Renk: Color
11. Kasa Tipi: Body Type
12. Kimden: Seller
13. Durum: Seller Status
14. KM: Kilometers
15. Fiyat: Price



It's a good idea to save these to a Python dictionary or in an external file, so we can look at them later without coming back here.

>Important: NaN values on the data shown as;
    1. Arac Tip: "-"
    2. Beygir Gucu: "Bilmiyorum"
    3. CCM: "Bilmiyorum"
