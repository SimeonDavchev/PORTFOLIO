
# PROJECT 2: Reservation Checker Automation

This project is centered around automating the process of checking and managing reservations across different platforms such as Booking.com, Expedia, and the proprietary website. The goal is to process reservation data and payment reports, and then to perform comparisons based on various criteria, like matching cancellations, prices, refunds, and more between platforms.

## Confidentiality NOTE:
To uphold the standards of data privacy and protection:
- Files are stored in a secure location with paths kept under `.gitignore`, which itself is hidden.
- Confidential data is only read from specified paths and is never displayed in the notebook. That is why the code with output that is in the public version has been commented out.
- Additional measures, such as hiding seeds and certain functions, will be implemented in future versions to further enhance confidentiality.

## PART I: Introduction and Remarks

The notebook sets the context by outlining the challenges faced in consolidating and managing reservations across platforms. Given the amount of reservations per week, it not only saves time (~2 hours by a conservative estimate), but it also emphasizes the need for automation to ensure accuracy, consistency, and efficiency in the reservation management process.

## PART II: Data Import and Preprocessing

This section delves into the initial phases of the data processing pipeline:
- Data is imported from various platforms, including Booking.com, Expedia, Hotel Tonight, and the proprietary website.
- The dataset from the proprietary website is further split into data from different platforms.
- Reservations from guests with multiple bookings are consolidated, ensuring that data comparisons are reliable and accurate.

## PART III: Data Analysis and Transformation

While the specific details and results are presented in the notebook, this section is dedicated to analyzing the processed data. The analysis aims to draw insights from the reservation trends, identify discrepancies, and ensure that the payment and reservation data aligns across platforms.

## Conclusion and Future Work
The Reservation Checker Automation streamlines the process of managing reservations from various platforms. It ensures data accuracy, reduces manual errors, and provides a comprehensive overview of reservation trends. Future iterations may expand towards other information of the reservations and provide useful analytics and insights from the information sourced.

