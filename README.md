AI Crop Recommendation Engine for SDG 2: Zero Hunger
This project is an AI-driven solution designed to address UN Sustainable Development Goal 2: Zero Hunger. It uses a machine learning model to recommend the optimal crop for farmers to plant based on their specific soil and environmental conditions.

The Problem (SDG 2)
Suboptimal crop selection is a major contributor to food insecurity and farmer poverty. Planting a crop unsuited to the local climate or soil composition leads to poor yields, wasted resources (water, fertilizer), and financial loss. This project aims to provide an accessible, data-driven tool to help farmers make smarter planting decisions.

The Solution: An AI-Powered Advisor
This project uses a Supervised Learning model (a Random Forest Classifier) to solve this problem.

Approach: Classification

Dataset: Crop Recommendation Dataset from Kaggle.

Features (Input): N (Nitrogen), P (Phosphorous), K (Potassium), temperature, humidity, ph, rainfall.

Label (Output): The recommended crop (e.g., 'rice', 'maize', 'coffee').

The model was trained on over 2,200 data points to learn the complex relationships between these environmental factors and optimal crop yield.

Project Demo
We can feed new environmental data into the model to get an instant recommendation.

Demo Input:

Nitrogen: 90

Phosphorous: 42

Potassium: 43

Temperature: 20.8°C

Humidity: 82%

pH Level: 6.5

Rainfall: 202.9 mm

Model Output:

✅ Recommended Crop: rice
Confidence: 100.00%

Model Performance
The model performs with extremely high accuracy, demonstrating its reliability in matching conditions to the correct crop. The confusion matrix below shows the model's predictions (x-axis) versus the actual true labels (y-axis). The strong diagonal line indicates outstanding precision and recall.

Overall Accuracy: 99.77%

Ethical & Social Reflection
Bias: This model is trained on a specific dataset. Its recommendations are biased towards the crops and regions in that data. It would likely perform poorly in a different continent and knows nothing of local, indigenous crops.

Accessibility: A Python script is not accessible to a rural farmer. To be fair and effective (SDG 10: Reduced Inequalities), this solution must be deployed through simple technology like SMS-based services or a voice-based app in local languages.

Sustainability: The model optimizes for yield, not long-term sustainability. It may recommend monoculture crops that deplete soil. A future version should be trained to recommend sustainable crop rotations.

This model is biased by its data, and it is inaccessible as a Python script. For this project to truly create a fitting solution, it can't just be smart; it must be fair and accessible. The next step would be to deploy this model not on a website, but through simple SMS or voice-based systems that work in any language, on any phone.

By linking AI to the SDGs, we can move from just writing code to building tools that can make a tangible difference in the fight against global hunger.
