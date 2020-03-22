# Sortierter Einkauf
**Project "SortierterEinkauf" for WirVsVirus Hackathon from 20.03.-22.03.2020**

WirVsVirus Hackathon: https://wirvsvirushackathon.org/

Project website: https://sortierteseinkaufen.de/

Project prototype app: https://sortierteseinkaufen.de/app/

# Project Description

**Motivation**

Hardly any other topic is as important to citizens in times of crisis as the supply of food. While social interaction should be avoided by necessity, shopping in the supermarket is essential for survival. 
We want to make our contribution by ensuring that citizens can buy all the products they need and that they are exposed to the lowest possible risk of infection when shopping (shopping distancing). In particular, ways to empty shelves in supermarkets are to be avoided to minimize unnecessary contact. To achieve these goals we offer a web app where a user can specify the products he needs. Supermarkets in the vicinity are then displayed, which, taking into account the inventory levels and current crowds, allow for a successful purchase with as little contact as possible. This relieves supermarkets, by a simplified coordination of visitor volumes and supports customers in their shopping.

**Approach and Solution**

When creating the solution, particular attention was paid to the fact that deployment should be possible very quickly. In this sense, it will enable supermarket customers to share the current stock of the market with the community. No user registration is required for this. The WebApp can be used directly and anonymously via any Internet-enabled device, e.g. smartphones or PCs.
Visitor numbers of the stores are recorded by a single, low-cost device in the entrance area of the supermarket. This IoT device is within a cost range of about 10-15€ and requires only a power connection for operation. After the central configuration of the devices, they are shipped to supermarkets. There is no further effort on site, the devices only need to be supplied with power. The device anonymously analyzes WLAN and Bluetooth data from present smartphones and thus enables a comprehensive evaluation of visitor numbers.

**Design Decisions and Rollout**

The WebApp prototype provided as part of the Hackathon, as well as all materials, can be scaled for large-scale deployment in just a few steps. Since no user and role administration needs to be integrated, the administrative effort is reduced to a minimum.
During the development of the solution, the use of dedicated hardware IoT devices was extensively discussed. Alternatives would include the use of Google or smartphone location data. However, it became apparent that up-to-date data on visitor numbers could only be accessed to a very limited extent via the Google API. Furthermore, costs are incurred here. The widespread use of smartphone user data poses numerous data protection hurdles. Furthermore, both possibilities increase the dependency on external sources. Since the presented IoT devices are inexpensive, quick and easy to use and provide reliable and accurate data, this option was chosen.

# Project Parts

The following project parts are contained in the prototype:

**Software-Frontend**

The frontend repository can be found at https://github.com/derpierre65/WirVsVirus-SortierterEinkauf-Frontend

**Software-Backend**

The backend repository can be found at https://github.com/engelant/WirVsVirus-SortierterEinkauf-Backend

**Hardware-IoT-Devices**

The proposed hardware IoT-devices are ESP-32 with LoRaWan connectivity.
To count the number of smartphones nearby via Bluetooth and Wifi sniffing, ESP Paxcounter (https://github.com/cyberman54/ESP32-Paxcounter) is used in it's default configuration. The devices are initialized with keys to communicate to The Things Network (https://www.thethingsnetwork.org/) via LoRaWan.

**Additional Information**

If you are looking for additional information for this project please refer to https://devpost.com/software/sortierteseinkaufen and https://sortierteseinkaufen.de/.

Teamwork from: Axel Wiepke, Adam Siwy, Jens Neureither, Daniel Demmer, Julian, Moritz, Florian, Ivan, Leon, Louis, Martin Münickel, Pierre Wüst, Andreas Bäuml

