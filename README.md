## Team Name: SMUrtNUS

  

*Team Members:*

  

Wong Hong Ming Bill - SMU Y1 Accountancy + Business Student

  

Ong Jia Le - SMU Y1 Information Systems Student

  

Liang Jia Wei Joshua - NUS Economics + Business Student

  

Wee Shaun - NUS Y1 Business Analytics Student

  

Lim Jin Hao - NUS Y1 Computer Science + Business Student

  
  

## What's the problem?

Currently in Singapore, there is a growing number of elderly living alone. This poses a serious problem as a significant number of deaths among the elderly recently are associated with domestic-related accidents such as falls, choking and cardiac arrests. SCDF works closely with Community First Responders (CFRs) to provide timely relief and response to emergency situations. With an increasingly aging population and a growing segment of vulnerable populations in mind (e.g. increasing trend of elderly with no next of kin), we require better sense-making for emergency services to be alerted at the onset of incidents which require emergency response (e.g. cardiac arrests, falls, unattended cooking fires etc.) and mobilise CFRs for effective early intervention especially to the vulnerable populations.

## How can technology help?

Fortunately, in the current digital age we are living in, there is a rising trend of elderly using smartphones. Hence, we could leverage on such trends to deliver help to the elderly digitally. Modern technologies such as those used in FitBit which helps track vital signs during exercises can be incorporated into our solution to help curb the problem we are facing.

## The idea


It is pivotal that emergency response measures can be improved and enhanced despite the growing rate of ageing population. Especially in times of COVID-19 situations where there is restriction of caregivers moving freely to person-at-risk houses frequently, this initiative which leverages IBM Cloud and Watson Services, will enable caregivers and emergency services to deliver help to the persons-at-risk at the most critical time as well as maintaining social responsibility.

  

Long Description

The SMUrtNUS initiative comprises two features: SMUrtNUS ring and SMUrtNUS mobile application.

Past and current data such as their age, past medication condition, etc. will be logged in by the user or with the help of their caregivers. This process will help to build a risk profile of the user. Before issuing the ring for the user to wear at home, there will be a trial phase for the user together with the guidance of the caregiver to normalise the predictive analytics to ensure that there are no glitches in the algorithm.

The SMUrtNUS ring is a wireless wearable connected to the SMUrtNUS Mobile Application. The person-at-risk has to wear the SMUrtNUS ring and download the SMUrtNUS Mobile Application on his/her phone. A caregiver will be tagged to the person-at-risk and they will also have the SMUrtNUS Mobile Application installed on their mobile phones as well. It will not require the person-at-risk to have much digital literacy. The ring is waterproof and fireproof to ensure that it will not spoil or be damaged easily. The ring will then monitor a user’s environmental data, such as their heart rate and temperature etc., and send them to the mobile application at an interval of every 5 minutes. The mobile application will be connected to a cloud server. Together with the user’s environmental data, their past and current data such as their age, past medication conditions, etc. will be processed using the IBM Auto A.I. software and used for predictive modelling for potential accidents, either cardiac arrest, fall or choking. When a potential accident has been predicted for a vulnerable person, their caregiver would be alerted through a notification from the mobile application, which would be followed up with a house call from the caregiver to the person-at-risk. If the person-at-risk does not pick up the call, the caregiver would alert the emergency services who will then deliver assistance to the person-at-risk. On the other hand, if the person-at-risk picks up the call from the caregiver, whether any assistance from emergency services is required would then depend on the condition of the person-at-risk. Ultimately, all potential incidents predicted by the A.I, whether requiring assistance or not from emergency services as the follow-up action, would be logged and recorded, before the data is sent back to the Auto A.I. This allows the A.I to progressively learn and refine the prediction model.

The emergency red button is a manual button which will alarm both the caregiver and hospitals in case the application happens to have technical difficulties, glitches. In the case of other accidents which have occurred falling outside of the modelled potential accidents (cardiac arrest, fall, choking) which would not be analysed and processed by the application, users will press the emergency red button to send emergency signals to the caregiver and hospitals.

If the phone battery is low, it will prompt the user to charge via the ring flashing red light and intermittent vibration. If the phone is not put to charge, the caretaker will get a notification message to ask the user to charge his phone.

  

Overall, the data consolidated from the mobile application will generate a risk profile for each user, which will then link the risk profiles to the gps function in smartphones to create a map of Singapore showcasing risk density areas. More caregivers will be efficiently allocated to the densely risk populated areas in Singapore.

## Demo video

[https://youtu.be/ndIcyUSlpFs](https://youtu.be/ndIcyUSlpFs)

  

## The Architecture

![](https://lh6.googleusercontent.com/PSmanP98bW8cIZC4CLTHv0tBl8MVOp9rSMMuNNM_878ODvQFE7LYQdM4CFR1UEuCSfrtBqJ5kBTAlt_BHMmM1un-9NElU9BI4nicOYoOa6IqtJBtckX1fuWZdIdW3vJcN1rOmxiI)

*Mechanism*

1.  Every 5 minutes, the SMartNUS ring will send environmental data such as heart rate and temperature to the SMartNUS mobile application. This will be our routine check.
    
2.  The data will then be sent to the ibm server to be passed to our prediction model built using IBM Auto A.I.
    
3.  The model will then analyse this data and make a prediction on whether there is an accident and if so, what type of accident will it be.
    
4.  If the model predicts an accident, the SMartNUS app will alert the caregiver and prompt him or her to contact the wearer.
    
5.  If the wearer picks up, they may decide to call 995 depending on the severity of the accident if it occurs. Or else, the caregiver should call 995 immediately.
    
6.  After the accident is taken care of, all data including the actual emergency type will be logged and recorded for refining the prediction model in the future.
    

 *Emergency Button* 

1.  The wearer can also directly trigger a manual emergency alert by pressing and holding the emergency button on the ring for 3 seconds.
    
2.  This manual alert will cause the SMartNUS app to simultaneously contact emergency services and the caregiver of a potential accident.
    
3.  The caregiver or the wearer may disable this alert through the SMartNUS app if it was unintentionally triggered.
    
4.  The data corresponding to the time of this incident, as well as the outcome will be also recorded into IBM’s cloud database to refine the prediction model. The automated A.I. will relearn every 2 weeks.
    

  

## Getting started

  

Setting up of profile: [https://smurtnus.mybluemix.net/ui/#!/0?socketid=TJdTfFNUtdtQjJ2SAAAu](https://smurtnus.mybluemix.net/ui/#!/0?socketid=TJdTfFNUtdtQjJ2SAAAu)

  

Disclaimer: This is an example of the prototype to illustrate our idea using the parameters of our app

  

The link above showcases an example of the setup of the elderly’s profile when their information is added into the system. Depending on the parameters of the data of each elderly which are updated on the system, a predicted accident (if any) will then be generated through the IBM Auto A.I. software.

  
  
  
  
  
  

## Evaluation

  

*Strengths*

  

1.  The SMUrtNUS ring is worn on the person-at-risk at all times which gives constant and timely updates to the caregiver
    
2.  Emergency red button to contact caregiver and garner attention if required, provides comprehensive coverage of accidents outside of the ones AI can predict: fall, cardiac arrest and choking
    
3.  The SMUrtNUS ring and SMUrtNUS mobile application’s functions are passive and do not require much involvement from the person-at-risk to function properly, hence even non tech-savvy persons-at-risk can utilise the ring and mobile application.
    

  

*Weaknesses*

  

1.  If the vulnerable person accidentally triggers the button while he is sleeping, and does not receive the phone call from the caregiver, a false alarm will be triggered
    
2.  Some vulnerable persons may not have a wifi connection for the data transmission to the server for the predictive service.


## Built With
*IBM Watson Auto A.I.* - Platform for prediction of data
*NodeRed* - Platform for building the testing interface
