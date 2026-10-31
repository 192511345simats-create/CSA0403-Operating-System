# TASK 12 – Re-evaluate and Adapt Operating-System Design

## Objective

To re-evaluate the proposed operating-system design for a smart hospital when new requirements, such as remote home monitoring and cloud-based patient records shared with partner hospitals, are introduced.

## Concept Details

This task focuses on adapting the existing smart hospital operating-system architecture to support new requirements.

The major concepts covered are:

1. Remote Patient Monitoring
2. Cloud-Based Patient Records
3. Distributed Operating Systems
4. Embedded Real-Time Operating Systems
5. Cloud Storage and Data Sharing
6. Network Communication
7. Security and Protection
8. Fault Tolerance and Reliability
9. System Scalability

## Design Decision

**Selected Approach: MODIFY**

The original smart hospital operating-system design is modified to support remote patient monitoring and cloud-based record sharing.

The existing architecture is retained wherever possible, while additional components are introduced to meet the new requirements.

## Modified Operating-System Architecture

| Environment             | Modified Design                      |
| ----------------------- | ------------------------------------ |
| Bedside Monitors        | Retain Hard Real-Time OS             |
| Nurses' Tablets         | Retain Handheld/Mobile OS            |
| Doctors' Workstations   | Retain Desktop OS                    |
| Hospital Database       | Expand to Distributed Cloud Database |
| MRI Systems             | Retain Multiprocessor OS             |
| Home Monitoring Devices | Introduce Embedded RTOS              |
| Partner Hospitals       | Expand Distributed Communication     |

## New System Features

### 1. Remote Home Monitoring

Home monitoring devices collect patient readings and process critical alerts locally.

### 2. Cloud-Based Patient Records

Patient records are securely stored in cloud-based infrastructure for authorized access.

### 3. Partner Hospital Communication

Authorized partner hospitals can access shared patient information through secure communication.

### 4. Local Processing

Critical alarms are processed locally without depending entirely on internet connectivity.

### 5. Offline Data Storage

Home monitoring devices temporarily store readings during network failures and synchronize them when connectivity returns.

## Security Considerations

* User authentication
* Role-based access control
* Encrypted communication
* Secure cloud storage
* Patient data privacy
* Authorized hospital access

## Reliability Considerations

* Local alarm generation
* Temporary data buffering
* Network failure handling
* Cloud backup
* Redundant infrastructure
* Recovery mechanisms

Cloud connectivity should not be treated as a guarantee of availability. Critical patient-monitoring operations must continue locally during internet or cloud-service failures.

## Impact on Original Design

| Original Design             | Modified Design                     |
| --------------------------- | ----------------------------------- |
| Monitoring inside hospital  | Hospital and home monitoring        |
| Central hospital records    | Cloud-supported distributed records |
| Hospital-only communication | Partner hospital communication      |
| Limited network dependency  | Expanded network connectivity       |
| Local patient information   | Secure shared patient information   |

## Software Requirements

* Assignment: CSA04 – CO1
* Topic: Operating-System Design Adaptation
* Reference Environment: Smart Hospital

## Files Included

| File Name              | Description                                               |
| ---------------------- | --------------------------------------------------------- |
| `README.md`            | Task description and design summary                       |
| `Task12_Answer.pdf`    | Complete theoretical explanation                          |
| `architecture.png`     | Modified smart hospital architecture diagram, if prepared |
| `comparison_table.png` | Original and modified design comparison, if prepared      |

## Result

The original smart hospital operating-system design was re-evaluated and modified to support remote patient monitoring, cloud-based records and secure information sharing with partner hospitals.

## Conclusion

Thus, the smart hospital operating-system design was successfully adapted to meet the new requirements. The modified architecture improves scalability and connectivity while maintaining local processing, patient safety, security and reliability.
