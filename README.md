# node-red-number-plate-recognition
Thir repository will have my flows for number plate recognition in node red<br>
![num plate reg](Number_plate_reg.png?raw=true "num plate reg")<br>
Install the following node

        node-red-contrib-plate-recognizer

register for free 2000 requests from web here https://app.platerecognizer.com/<br>
Get Token and update node with your token

## Here is test code to see if your token work

    curl -o /tmp/car.jpg https://app.platerecognizer.com/static/demo.jpg # Get an image
    curl -F "upload=@/tmp/car.jpg" -F regions=us-ca \
    -H "Authorization: Token yout token here" \
    https://api.platerecognizer.com/v1/plate-reader
