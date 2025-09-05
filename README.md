# AUTOMATIC-RAILWAY-TRACK-CRACK-DETECTOR

The Indian Railway has one of the largest railway networks in the world, covering over 1,15,000 km. A recent study found that more than 25% of the track length needs replacement because of cracks. Detecting cracks manually is difficult and not very effective.

This project aims to solve the problem by developing an automatic railway track crack detection system. The system uses an infrared (IR) crack sensor along with GSM technology to send information about the crack’s location to a central station. This allows maintenance staff to respond quickly.

The system is built with several components: GSM module, GPS receiver, Arduino board, GPS antenna, IR sensor, battery, and DC motor. The Arduino board is the main platform, and it is programmed to connect with both the GSM and GPS modules.

The GPS helps to find the exact location of the crack by providing latitude and longitude. The GSM module sends this information as a message to the nearest station or maintenance center.

This project is fully automated, meaning it does not need human effort to detect cracks. Automation reduces manual work, increases efficiency, improves accuracy, and saves time.

The main benefits of automation are:

Reduces manpower

Increases system efficiency

Decreases workload

Provides higher accuracy

Saves time

Reduces worker fatigue

Prptotype Image

![IMG_20190812_105636](https://github.com/user-attachments/assets/161f567b-c271-481c-b36c-184d8ba18e7d)

![IMG_20190812_104820](https://github.com/user-attachments/assets/4d1c87dd-1edd-44da-b200-24fc3559372b)

Working Principle of the System

The proposed project employs two sets of Infrared (IR) sensor units mounted on both sides of the vehicle. These sensors continuously monitor the condition of the railway track and serve as the primary input to detect cracks. The sensing mechanism is directly linked to a GSM communication module, which transmits alerts to a mobile device when a crack is detected. The overall working can be divided into two modes:

A. Normal Operating Condition

The IR transmitter continuously emits infrared rays, which are detected by the corresponding IR receiver positioned on the same side of the vehicle.

Both sensor units (one on each side of the track) function simultaneously to ensure complete monitoring.

When the track is intact, both sensors receive uninterrupted signals. This condition is interpreted as Low–Low (0–0) by the circuit.

In this case, the vehicle proceeds normally along the track without interruption, as no abnormality is detected.

B. Crack Detection Condition

If a crack appears on either side of the track, the infrared signal is interrupted for that particular sensor.

The affected sensor outputs a High signal (1), while the other remains Low. This discrepancy is detected by the interfacing Integrated Circuit (IC).

The IC processes the signal and triggers the relay driver circuit, which in turn notifies the microcontroller of the fault condition.

The microcontroller then commands the GSM module to send an alert message to the pre-configured mobile number, providing real-time information about the detected crack.

This ensures that corrective action can be taken immediately to prevent accidents or derailments.

Conclusion

The automatic railway track crack detection system provides a reliable and efficient solution to ensure railway safety. By integrating IR sensors, GPS, and GSM technology with Arduino, the system can automatically detect cracks, identify their exact location, and immediately send alerts to the maintenance team. This reduces manual effort, saves time, and improves the accuracy of fault detection. In the long run, such automation helps in preventing accidents, reducing maintenance costs, and increasing the overall efficiency of railway operations.
