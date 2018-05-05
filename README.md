# Python-Programming-Beginning-la.weather.csv
weather_data=[]
f=open("la_weather.csv","r")
data=f.read()#the file is made of two components:the days and the weather type
rows=data.split("\n")
for i in rows:
    split_row=i.split(",")
    weather_data.append(split_row)
    
weather = []
for i in weather_data:
    value=i[1]
    weather.append(value)#this step only retrieves the weather type and store them into the weather list
count=0
for i in weather:
    count=count+1#tally the total numbers
new_weather=[]
new_weather=weather[1:len(weather)]#remove the header

#animals = ["cat", "dog", "rabbit"]
#for animal in animals:
    #if animal == "cat":
        #print("Cat found")
        
#animals = ["cat", "dog", "rabbit"]
#if "cat" in animals:
    #print("Cat found")
    
#animals = ["cat", "dog", "rabbit"]
#cat_found = "cat" in animals



