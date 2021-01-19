### These programs calculated an NAO index that is normalized by its standard deviation. 

However, I noticed something weird about the normalization. When I take a moving average of the anomalies, then normalize that moving average by its standard deviation, I get something like the following (this is just one ensemble member of one model):
<img width="1304" alt="Screen Shot 2021-01-19 at 5 18 58 PM" src="https://user-images.githubusercontent.com/69660053/105100201-f05bf380-5a7a-11eb-9781-216b8fe74ec0.png">
On the other hand, when I normalize the anomalies before taking the moving average of that normalized anomaly data, I get something like this:
<img width="1276" alt="Screen Shot 2021-01-19 at 5 19 21 PM" src="https://user-images.githubusercontent.com/69660053/105100386-3e70f700-5a7b-11eb-96d5-62ef7868ca4e.png">
It's the same qualitative pattern but a different amplitude. I'm not sure which method is better. I based the normalization on a figure in Chapter 3 of Arin Nelson's PhD thesis, and the former figure looks more similar to what he has. However, according to Baylor, the normalization Arin was doing was specifically useful for his project but not currently necessary for what I'm doing. Thus I am creating versions of the code in this folder that don't normalize the data.
