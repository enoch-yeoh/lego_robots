# lego_robots
Lego Boost has been discontinued. The app is still available, but there has been some enthusiasts that have some open source code.
here is one of them:
https://legoboost.azurewebsites.net/

a basic code
import LegoBoost from 'lego-boost-browser';

const boost = new LegoBoost();

async () => {
await boost.ledAsync('green');
    
    // Use motor angle control for precise movement
    await boost.motorAngleMultiAsync(360, 50, 50); // Both motors 360 degrees at 50% power
    
    await boost.ledAsync('yellow');
    
    // Turn using different motor speeds
    await boost.motorAngleMultiAsync(180, 30, -30); // Turn by running motors in opposite directions
    
    await boost.ledAsync('red');
    
    // Move back
    await boost.motorAngleMultiAsync(360, -50, -50); // Reverse direction
    
    await boost.ledAsync('blue');
}

controlled via Bluetooth from the phone
https://youtube.com/shorts/M3TDImQZDzc

There are other projects like line tracing, which was done with separate robots and modules, using 1 and 2 light sensors.


