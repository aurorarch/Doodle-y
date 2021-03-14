# Doodle-y
Everyone has played Skribble once in their life. What about teaching machines to guess the correct doodles?

## Description
Google's [Quick Draw](https://quickdraw.withgoogle.com/) project asked users to draw rough sketches of regular objects in order to train them on neural networks, to teach the machine to recognise them correctly. This game is similar to the now-a-days popular online game 'Skribble'. To know more, check their [github repo](https://github.com/googlecreativelab/quickdraw-dataset).

## Dataset
They created the data from the users which they preprocessed in various form. It can be found on their github repo. Feel free to choose any format you like to work with.
I got the ```.npy``` file from [here](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap;tab=objects?prefix=&forceOnObjectsSortingFiltering=false)

The classes that I chose were:
1. Airplane
2. Bicycle
3. Bear
4. Cake
5. Moon
6. Calendar
7. Calculator
8. Dragon
9. Door
10. Fan
11. Fish
12. Candle
13. Lion
14. Snowflake

There are approx 350 classes. Take as many as you want.

## Steps for Colab
1. Go to [Google Cloud](https://console.cloud.google.com/) and create a new project.
2. Run these lines.
    ```
    !curl https://sdk.cloud.google.com | bash
    ```
    ```
    !gcloud init
    ```
3. Fill the info about your account. *Creating a new project in cloud is necessary to download the data*.
4. Train the data and save the model.
