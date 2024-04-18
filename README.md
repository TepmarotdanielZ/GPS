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

![image_2024-04-04_11-40-15](https://github.com/TepmarotdanielZ/GPS/assets/139426571/46ec762d-c0b7-4108-bd26-24599467494f)

    . DMA:

![Screenshot from 2024-04-18 15-32-05](https://github.com/TepmarotdanielZ/GPS/assets/139426571/a24d6681-4ce6-4f98-9c60-a35ae7b249bc)
