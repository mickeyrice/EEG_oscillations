# EEG_oscillations
Using machine learning to predict sleep patterns in a publicly available EEG dataset from the Challenge data initiative. 
From website:
https://challengedata.ens.fr/professors/challenges/10/
Challenge context

Measuring Sleep
The measurment of sleep is usually done in a sleep laboratory. Various electrods are attached to the head to measure physiological signals. Electrical activity in the brain is measured by electroencephalography (EEG). Muscle activity is recorded using electromyography (EMG), because muscle tone also differs between wakefulness and sleep. Eye movements during sleep are measured using electro-oculography (EOG). Other sensors can be added (pulseoxymeter, airflow etc.) These procedure is called polysomnographie (PSG) and allows to analyse the state of the patient during sleep. It also allows to track sleep related disease such as sleep apnea or restless-leg syndrom.

Dreem Headband
Dreem headband is a device able to measure sleep at home. It is easy to use and confortable compared to a classic PSG. Its aims to help people track and improve their sleep. The Dreem headband uses three kind of sensors: EEG electrods, accelerometer and pulseoximeter. Hence, it is able to measure brain activity, position, respiration, heartrate and movement all along the night. The device is also able to send sounds using bone conduction. Signals are analyzed online throughout the night and the device is able to perform sound stimulation to enhance deep sleep quality at different steps of the night : falling asleep, deep sleep and awakening. More info at dreem.com/product.

Context
In this challenge, data consists on EEG signals acquired on the Dreem headband in sham condition i.e. without any kind of sound stimulations. Thus we aim to predict brain activity in normal condition.

Challenge goals
Normal sleep
Sleep progresses in cycles that involve multiple sleep stages : wake, light sleep, deep sleep, rem sleep. Different sleep stages are associated to different physiological functions. The represenation of the sleep stages through the night is called an hypnogram and is built from the physiological signals recorded by PSG and analyzed by window of 30seconds.Hypnogram

Deep Sleep
Deep sleep (also called slow wave sleep) occurs mainly in the first hours of sleep. It is associated with memory consolidation, energy restoration, hormone releasing. Electroencephalographic measurement in deep sleep is characterized by slow oscillations: trains of high magnitude and low frequency waves (1-4 Hz).

Deep sleep enhancement
Deep Sleep can be enhanced by inducing slow oscillations through various kind of stimulations (auditory, visual, magnetic etc. see this publication). The Dreem headband is able to perform such sound stimulation during deep sleep.

Goals
In this dataset, we try to predict whether or not a slow oscillation will be followed by another one in sham condition, i.e. without any stimulation. This will allow to:

Predict normal brain activity
Know when it’s interesting to stimulate
Better quantify the impact of an individual stimulation by comparing to what would have occurred without stimulation.

Update 4/14: ML algorithm has not been optimized yet, still need to try new algorithms.
