# Machine Intelligence Project - UE20CS302
<h2>Ventilator pressure prediction</h2>
<body>
This project deals with time series analysis, to predict pressure of a mechanical ventilator for a given patient.
<p>The dataset required for this project has been taken from <a href = "https://www.kaggle.com/competitions/ventilator-pressure-prediction/overview">Kagggle</a></p>

<h2>Dataset Overview</h2>
<p>The following are the features of the dataset
<ol>
<li>  id - globally-unique time step identifier across an entire file</li>
<li>  breath_id - globally-unique time step for breaths</li>
<li>  R - lung attribute indicating how restricted the airway is (in cmH2O/L/S). Physically, this is the change in pressure per change in         flow (air volume per time). Intuitively, one can imagine blowing up a balloon through a straw. We can change R by changing the               diameter of the straw, with higher R being harder to blow.
</li>
<li>  C - lung attribute indicating how compliant the lung is (in mL/cmH2O). Physically, this is the change in volume per change in               pressure. Intuitively, one can imagine the same balloon example. We can change C by changing the thickness of the balloon’s latex,           with higher C having thinner latex and easier to blow.</li>
<li>  time_step - the actual time stamp.</li>
<li>  u_in - the control input for the inspiratory solenoid valve. Ranges from 0 to 100.</li>
<li>  u_out - the control input for the exploratory solenoid valve. Either 0 or 1.</li>
<li>  pressure - the airway pressure measured in the respiratory circuit, measured in cmH2O.</li>


</ol
</p>
</body>

<h2>Model Used</h2>
<p>Given the depth of Data and time series nature, I've followed Deep Learning methodology for this project.
An ANN Sequential model using TensorFlow Keras has been implemented for this project.
For the model creation,I have used <ul><li> 25 hidden layers</li> <li>50 units in each layer</li> <li> 300 epochs</li></ul>
<p>Then final MAE(Mean Absolute Error) for this has found to be 0.5403</p>
</p>

