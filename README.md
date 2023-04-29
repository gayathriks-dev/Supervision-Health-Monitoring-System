# Supervision-Health-Monitoring-System

In the standard of living, corporate and industry workers dwindle to have a health-work balance. As technology advances, AI and Machine learning contribute to our health sector. Using Artificial neural network - a Deep learning algorithm for medical management, providing prolific endeavours in elucidating these complications on medical management by monitoring vital parameters daily by AI-based health care assist. And furthermore, helping people to have regular health check-ups to help provide diagnosis at an early stage, and avoiding the development of chronic illness provides benefits for both corporate and industry workers and the industry.

1. With the help of the sensors such as a Foot pressure sensor, Pulse oximeter,
GSR and Temperature sensor we are getting the person's vital parameters and
all the sensors are connected to the Arduino board.

1. The inputs from the Arduino board are compiled using Arduino ide and the
inputs are converted into python inputs using the python test code.
                    mv = ( temperature value/1024.0)*5000
                    cel = mv/10
                    farh = (cel*9)/5 + 32
                    gsrvoltage = gsrsensorvalue * (5.0 / 1023.0)
                    res = -2 * gsrvoltage + 10; //y = -2x + 10
                    con = 1 / res
                    stress = -(-20 * res + 100); //y = -20x + 100
                    footsensorvoltage1 = footsensorvalue1 * (5.0 / 1023.0)
                    footpress1 = 222.22 * footsensorvoltage1; //y = 222.22x
2. Initially, the inputs are in the form of strings, then convert the string input to
the array input in order to use the inputs in the streamlit, where the streamlit
is used for creating the front-end of the application.

3. The inputs are processed and if the input values are greater than the
threshold values then the person is abnormal and if the inputs are lesser than
the threshold value then the person is normal

4. The results of the person's normalization status will be displayed in the front
end.
![athena](https://user-images.githubusercontent.com/95515002/235286200-9de07f44-6507-44c8-858d-ac2782bd4ba1.png)

![Screenshot 2022-10-27 212505](https://user-images.githubusercontent.com/95515002/235286262-6b2c9fdf-736e-4843-8e3f-d64a8e518b1a.png)
![Screenshot 2022-10-27 212046](https://user-images.githubusercontent.com/95515002/235286263-67f03240-8eae-481a-ad9a-cae10b19814c.png)

