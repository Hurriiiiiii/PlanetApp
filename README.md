This Android project demonstrates how to create a fully customized ListView using:

A model class (Planet)
A custom ArrayAdapter (MyCustomAdapter)
A custom row layout (item_list_layout.xml)
Planet images + moon count displayed for each item
Click events using OnItemClickListener
The app displays a list of planets along with:
Planet Name
Number of Moons
Image of the Planet
When the user taps a planet, the app shows a Toast displaying the selected planet’s name.
This project is ideal for learning custom adapters, model classes, and efficient view handling using the ViewHolder pattern.

🌟 Features

✔ Custom ListView with images
✔ Uses a Planet model class
✔ Custom Adapter extends ArrayAdapter<Planet>
✔ Efficient scrolling using ViewHolder pattern
✔ Click listener on list items
✔ Clean UI layout using ConstraintLayout

🧩 How It Works
1️⃣ Model Class — Planet.java
Defines:
planetName
moonCount
planetImage (int → drawable resource)
Encapsulates data for each list item.

2️⃣ Custom Adapter — MyCustomAdapter.java
Extends ArrayAdapter<Planet>
Inflates item_list_layout.xml
Binds:
Image
Planet name
Moon count
Implements ViewHolder pattern for smooth list performance.

3️⃣ MainActivity
Creates an ArrayList<Planet>
Adds planets with name, moon count, drawable image
Binds custom adapter to ListView
Handles item click to show a Toast

4️⃣ Custom Row Layout — item_list_layout.xml
Displays:
Planet image
Planet name
Moon count
Neat and spaced UI using ConstraintLayout.

5️⃣ Activity Layout — activity_main.xml

Contains only the ListView filling the screen.

📦 File Structure

    /java/com/example/planetapp
    │── MainActivity.java
    │── MyCustomAdapter.java
    │── Planet.java

    /res/layout
    │── activity_main.xml
    │── item_list_layout.xml

    /res/drawable
    │── earth.png
    │── mars.png
    │── venus.png
    │── etc…
