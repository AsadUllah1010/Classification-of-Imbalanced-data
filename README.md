# Classification-of-Imbalanced-data
In Machine Learning, imbalanced data refers to a situation in classification problems where the number of observations in each class significantly differs. In such datasets, one class (the majority class) vastly outnumbers the other class (the minority class).
# Introduction
The imbalance can lead to biased models that favour the majority class, resulting in poor predictive performance on the minority class, which is often the class of greater interest. Handling imbalanced data in classification tasks is a challenge that requires careful consideration of data preprocessing, resampling strategies, model choice, and evaluation metrics. Below is the process you can follow while performing classification on imbalanced datasets:
1. Begin by analyzing the distribution of classes within your dataset to understand the extent of the imbalance.
2. Determine the importance of each class in the context of your specific problem.
3. Increase the number of instances in the minority class by replicating them to balance the class distribution.
4. Some algorithms, like tree-based methods, are less sensitive to class imbalance. Consider using these or ensemble methods like Random Forest or Gradient Boosted Trees.
5. Besides accuracy, use metrics that are informative for imbalanced datasets, such as Precision, Recall, F1 Score, or the Area Under the Receiver Operating Characteristic (AUROC) curve.
# Features
In the insurance industry, predicting the likelihood of claims is critical for risk assessment and policy pricing. However, insurance claims datasets often exhibit class imbalance, with non-claims outnumbering actual claims. This imbalance can lead to predictive models that are biased towards the majority class, resulting in poor predictive performance for the minority class, which is often of greater interest.
The given dataset contains the following features:
1. policy_id: Unique identifier for the insurance policy.
2. subscription_length: The duration for which the insurance policy is active.
3. customer_age: Age of the insurance policyholder, which can influence the likelihood of claims.
4. vehicle_age: Age of the vehicle insured, which may affect the probability of claims due to factors like wear and tear.
5. model: The model of the vehicle, which could impact the claim frequency due to model-specific characteristics.
6. fuel_type: Type of fuel the vehicle uses (e.g., Petrol, Diesel, CNG), which might influence the risk profile and claim likelihood.
7. max_torque, max_power: Engine performance characteristics that could relate to the vehicle’s mechanical condition and claim risks.
8. engine_type: The type of engine, which might have implications for maintenance and claim rates.
9. displacement, cylinder: Specifications related to the engine size and construction, affecting the vehicle’s performance and potentially its claim history.
10. region_code: The code representing the geographical region of the policyholder, as claim patterns can vary regionally.
11. region_density: Population density of the policyholder’s region, which could correlate with accident and claim frequencies.
12. airbags: The number of airbags in the vehicle, indicating safety level which can influence claim probability.
13. is_esc (Electronic Stability Control), is_adjustable_steering, is_tpms (Tire Pressure Monitoring System): Features that enhance vehicle safety and could potentially reduce the likelihood of claims.
14. is_parking_sensors, is_parking_camera: Parking aids that might affect the probability of making a claim, especially in urban areas.
15. rear_brakes_type: Type of rear brakes, which could be related to the vehicle’s stopping capability and safety.
16. Features like steering_type, turning_radius, length, width, gross_weight, and various other binary indicators (Yes/No) for specific vehicle amenities and safety features, which together build a profile of the vehicle’s characteristics and its associated risk factors.
17. claim_status: Indicates whether a claim was made (1) or not (0), which is the dependent variable the model aims to predict.
<br>
Your task is to develop and evaluate a predictive model that accurately identifies the likelihood of insurance claims, despite the inherent class imbalance in the dataset. The model should maintain high predictive accuracy across both classes, ensuring that insurers can effectively assess risk and allocate resources.

