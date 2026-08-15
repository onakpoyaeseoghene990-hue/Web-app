# Fuel Freely Master UI/UX Prompt - Part 1B
==================================================
MASTER UI/UX PROMPT — PART 1B
Fuel Freely (Responsive AI-Powered Nutrition Web Application)
==================================================

--------------------------------------------------

DASHBOARD

The Dashboard is the primary workspace of Fuel Freely. It should provide users with an immediate, easy-to-understand overview of their nutritional progress, meal activity, health insights, and personalized recommendations.

The layout must prioritize the most important information first while minimizing cognitive load.

Dashboard Sections

1. Daily Nutrition Overview

Display a fuel gauge-inspired progress ring showing

• Calories Consumed

• Calories Remaining

• Daily Goal

The progress ring should visually reinforce the Fuel Freely brand while remaining easy to interpret.

--------------------------------------------------

2. Macronutrient Overview

Display a pie chart illustrating the user's daily macronutrient distribution.

Include

• Protein

• Carbohydrates

• Fat

When users hover over or select a chart segment, display

• Current intake

• Recommended intake

• Remaining target

--------------------------------------------------

3. BMI Summary

Display the user's current Body Mass Index.

Include the disclaimer

"BMI is a general health indicator and does not account for muscle mass or overall body composition."

--------------------------------------------------

4. Quick Statistics

Display concise summary cards for

• Meals Logged Today

• Remaining Calories

• Calories Burned

• Water Intake

• Current Nutrition Goal

Each card should provide a clear value and a short description.

--------------------------------------------------

5. Nutrition Insights

Generate personalized insights based on the user's recent eating habits.

Examples

• Your protein intake has improved this week.

• Consider increasing fibre during dinner.

• Your calorie intake has remained consistent over the last seven days.

Keep recommendations positive, practical, and actionable.

--------------------------------------------------

6. Recommended Meals

Recommend meals that align with

• Remaining calories

• Macronutrient targets

• Allergies

• Food intolerances

• Dietary requirements

• Preferred cuisine

Recommendations should remain culturally relevant and realistic.

--------------------------------------------------

7. Reminder Cards

Display reminders for

• Completing onboarding

• Drinking water

• Logging meals

• Reviewing nutrition progress

Allow users to dismiss reminders individually.

--------------------------------------------------

8. Notifications

Display recent notifications including

• Nutritionist messages

• Meal reminders

• Recommendation updates

• Application announcements

Unread notifications should be visually distinguishable.

--------------------------------------------------

CUISINE PREFERENCE

Provide a persistent cuisine selector.

Options

• Nigerian Cuisine

• International Cuisine

Automatically select the default cuisine based on the user's preferred language while allowing manual changes before each meal entry.

Remember the most recently selected cuisine.

--------------------------------------------------

MEAL LOGGING

Support three meal logging methods.

Every method must conclude with a confirmation screen before the meal is permanently saved.

--------------------------------------------------

IMAGE LOGGING

Workflow

Choose Cuisine

↓

Upload Meal Image

or

Capture Image Using Webcam

↓

AI analyzes the uploaded image.

↓

Return two or three possible meal matches together with confidence scores.

↓

The user selects the correct meal.

↓

Retrieve nutritional values from the USDA FoodData Central API whenever an equivalent food exists.

If no equivalent food exists, clearly indicate that nutritional values are estimated and allow the user to confirm the meal before saving.

↓

Display

• Estimated Calories (Range)

• Protein

• Carbohydrates

• Fat

• Fibre

• Serving Size

↓

Save the confirmed meal to Meal History.

--------------------------------------------------

TEXT ENTRY

Workflow

Choose Cuisine

↓

Display commonly logged meals.

↓

Allow instant search.

↓

Allow manual meal entry.

↓

If the selected meal belongs to a food family, display all relevant variations.

Example

Jollof Rice

↓

Party Jollof

↓

Homemade Jollof

↓

Village Jollof

↓

User confirms the selected meal.

↓

Retrieve nutritional values from the USDA FoodData Central API whenever an equivalent food exists.

If no equivalent food exists, clearly label nutritional values as estimated before allowing the user to save the meal.

↓

Display nutritional summary.

↓

Save meal.

--------------------------------------------------

VOICE LOGGING

Workflow

Choose Cuisine

↓

Record Voice

↓

Use the Browser Web Speech API (SpeechRecognition) where supported.

↓

Convert speech to text.

↓

If speech recognition is unavailable, allow users to upload an audio recording for server-side transcription.

↓

AI analyzes the meal description.

↓

Return two or three possible meal matches together with confidence scores.

↓

User confirms the detected meal.

↓

Retrieve nutritional values from the USDA FoodData Central API whenever an equivalent food exists.

If no equivalent food exists, clearly indicate that nutritional values are estimated before allowing the user to save the meal.

↓

Display nutritional summary.

↓

Save meal.

The first time Voice Logging is used, display a one-time example demonstrating how users should naturally describe a meal.

Example

"I ate one serving of jollof rice with grilled chicken and a small bottle of orange juice."

--------------------------------------------------

MEAL CONFIRMATION

Before saving any meal, display a confirmation page containing

• Meal Name

• Meal Image (if available)

• Estimated Calories

• Macronutrients

• Serving Size

• Detected Allergens

• Detected Food Intolerances

• Confidence Score

Allow users to

• Edit the meal

• Change the serving size

• Select another AI suggestion

• Cancel

• Confirm and Save

No meal should be permanently stored without explicit user confirmation.

--------------------------------------------------

FAVOURITES

Display

• Frequently Logged Meals

• Recent Meals

• Pinned Meals

Allow users to

• Pin meals

• Rename favourites

• Remove favourites

• Log a favourite meal with one click

--------------------------------------------------

GLOBAL SEARCH

Provide a persistent search bar accessible throughout the application.

Allow users to search

• Meals

• Ingredients

• Meal History

• Favourite Meals

• Nutrition Recommendations

• Recently Logged Meals

Display autocomplete suggestions while typing.

Rank results according to

• Relevance

• Frequently Logged Meals

• Recent Activity

• User Preferences

--------------------------------------------------

API BEHAVIOUR

Firebase Authentication

Use Firebase Authentication to

• Register users

• Authenticate users securely

• Reset passwords

• Verify email addresses

• Maintain authenticated sessions

--------------------------------------------------

Firebase Firestore

Store

• User Profiles

• Meal History

• Nutrition History

• Dashboard Preferences

• Dietary Requirements

• Allergy Information

• Notification Preferences

• Favourite Meals

• Recent Meals

--------------------------------------------------

USDA FoodData Central API

Retrieve

• Calories

• Macronutrients

• Micronutrients

• Serving Sizes

• Food Descriptions

Whenever an exact food match is unavailable, clearly inform users that displayed nutritional values are estimated and allow them to confirm the meal before saving.

--------------------------------------------------

LibreTranslate API

Translate

• Dashboard Labels

• Notifications

• Educational Content

• Recommendations

• System Messages

Always preserve user-entered food names to avoid incorrect translations.

--------------------------------------------------

Firebase Cloud Messaging

Deliver notifications generated by the application.

Examples include

• Meal Reminders

• Daily Nutrition Summaries

• Nutritionist Notifications

• Recommendation Alerts

• Weekly Progress Updates

Allow users to enable or disable each notification category individually.

--------------------------------------------------

END OF PART 1

