# 1. GPS 

# TEST GPS NEO M8N

This tutorial will cover the Interfacing of the GPS Module (Neo 6M) with the STM32. We will see how we can get the location, time, date, speed, altitude etc.

![image](https://github.com/TepmarotdanielZ/GPS/assets/139426571/f7794236-98c7-456c-a7c8-b0aab4d12fe6)

As we are going to use the UART for the data transmission, also the length of the data is unknown, This tutorial is going to use the UART Ring Buffer from one of my previous Posts. It is recommended that you first go through that tutorial, and make it work.
The GPS module Transmits the data via the UART in the NMEA format. In this tutorial, we will see how to decode it and extract the useful information from this data. The sample data in the NMEA format is shown below.

# 2. CONFIGURATION 

    . RCC:

![Screenshot from 2024-04-18 15-26-10](https://github.com/TepmarotdanielZ/GPS/assets/139426571/c00ae298-6646-4a16-aa7f-d4bc0076387b)

    . SYS:

![Screenshot from 2024-04-18 15-27-23](https://github.com/TepmarotdanielZ/GPS/assets/139426571/8117b2d0-e7de-413f-a262-e6af00f1a107)

    . CLOCK:

![Screenshot from 2024-04-18 15-28-07](https://github.com/TepmarotdanielZ/GPS/assets/139426571/f6c1f662-2274-4353-a96a-82252d2b12cf)

    . USART2:

![Screenshot from 2024-04-18 15-29-37](https://github.com/TepmarotdanielZ/GPS/assets/139426571/bf4833bc-3bfc-40e6-995b-bb12848e91c8)

    . NVIC:

![Screenshot from 2024-04-18 15-30-52](https://github.com/TepmarotdanielZ/GPS/assets/139426571/2bf17bac-dafb-4838-9ae5-c7c3cd1c3ba7)

    . DMA:

![Screenshot from 2024-04-18 15-32-05](https://github.com/TepmarotdanielZ/GPS/assets/139426571/a24d6681-4ce6-4f98-9c60-a35ae7b249bc)

# 4. CODE  

![Screenshot from 2024-04-18 15-36-52](https://github.com/TepmarotdanielZ/GPS/assets/139426571/1dfc0d86-4c15-41af-a076-4db49d9dfec0)

![Screenshot from 2024-04-18 15-37-20](https://github.com/TepmarotdanielZ/GPS/assets/139426571/751f7d7c-f684-47d6-85fe-6bdcd600d846)

![Screenshot from 2024-04-18 15-37-41](https://github.com/TepmarotdanielZ/GPS/assets/139426571/a6b1dedb-b713-4172-b671-322cc17bb0f8)

# 5. INCLUDE LIBRARY (lwgps.h)

![Screenshot from 2024-04-18 15-39-55](https://github.com/TepmarotdanielZ/GPS/assets/139426571/db559f12-f3c9-4dba-aa32-001a93b816c3)

# 6. INCLUDE LIBRARY (lwgps.c)

![Screenshot from 2024-04-18 15-40-02](https://github.com/TepmarotdanielZ/GPS/assets/139426571/bf1de43f-d85f-40a4-810f-b97ad180a787)

# 7. SCEMATIC DAIGRAM 

![image_2024-04-04_11-40-15](https://github.com/TepmarotdanielZ/GPS/assets/139426571/46ec762d-c0b7-4108-bd26-24599467494f)

# 8. RESULT TESTING GPS

![image](https://github.com/TepmarotdanielZ/GPS/assets/139426571/3a2aaa60-da8b-4e7c-bb93-586bb0990e4c)

![image](https://github.com/TepmarotdanielZ/GPS/assets/139426571/c9fa2b87-8660-4a22-a68d-f0c8ddadab87)




