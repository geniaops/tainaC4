### <span style="color:red">NOTE: This repo is being updated daily.</span>

# TAINA Voice AI System Documentation

Welcome to the comprehensive documentation for the TAINA Voice AI system. This repository contains architectural, project management, design, testing, data collection, and deployment documentation that supports the "IA para la Ciudadanía" initiative.

## Project Context

The "IA para la Ciudadanía" project aims to develop an AI-based citizen interaction system that centralizes data collection and processing through intelligent kiosks ("ventanillas inteligentes"). TAINA serves as the voice-enabled AI assistant that provides government service information, personalized recommendations, and assistance to citizens across multiple channels.

## Documentation Structure
<!-- 
0. [Client Requirements](./0_Plan.md) ✅ *Complete*
1. [Documentation Gap Analysis and Implementation Plan](./1_Documentation_Gap_Analysis_and_Implementation_Plan.md) ✅ *Complete*
2. [Architecture Documentation](./2_Architecture/) 🔜 *Coming soon*
    -C4 ⏳ *In progress*
    - 2.1. [Product Backlog](./2_Architecture/c4-model/2.1_Context_Diagram.md) ✅ *Complete*
4. [Project Management Documentation](./3_Project_Management/) 🔜 *Coming soon*
    -Backlog
    - 3.8. [Product Backlog](./3.8_Product_Backlog_TAINA.md) ✅ *Complete*
    - 3.8. [Product Backlog](./3_Project_Management/backlog/3.8_Product_Backlog_TAINA.md) ✅ *Complete*
5. [Design Documentation](./4_Design/) 🔜 *Coming soon*
6. [Testing Documentation](./5_Testing/) 📝 *Planned*
7. [Implementation Documentation](./6_Implementation/) ⏳ *In progress*
8. [Data Collection and Analysis Documentation](./6_Data_Collection_and_Analysis/) 📝 *Planned*
9. [Deployment Documentation](./7_Deployment/) 📝 *Planned*
-->

0. [Client Requirements](./0_Plan.md) ✅ *Complete*
1. [Documentation Gap Analysis and Implementation Plan](./1_Documentation_Gap_Analysis_and_Implementation_Plan.md) ✅ *Complete*
2. [Architecture Documentation](./2_Architecture/) 🔜 *Coming soon*
    - C4 <!--(./2_Architecture/c4-model/)--> ⏳ *In progress*
      - 2.1. [Context Diagram](./2_Architecture/c4-model/2.1_Context_Diagram.md) 📄 *Published (under revision)*
3. [Project Management Documentation](./3_Project_Management/) 🔜 *Coming soon*
    - 3.7 Project Roadmap [Project Roadmap](./3_Project_Management/backlog/3.7_Project_Roadmap.md)
    - Backlog <!--(./3_Project_Management/backlog/)--> ⏳ *In progress*
      - 3.8. [Product Backlog](./3_Project_Management/backlog/3.8_Product_Backlog_TAINA.md) ✅ *Complete*
6. [Design Documentation](./4_Design/) 🔜 *Coming soon*
7. [Testing Documentation](./5_Testing/) 📝 *Planned*
8. [Implementation Documentation](./6_Implementation/) ⏳ *In progress*
9. [Data Collection and Analysis Documentation](./6_Data_Collection_and_Analysis/) 📝 *Planned*
10. [Deployment Documentation](./7_Deployment/) 📝 *Planned*

## System Overview

The TAINA Voice AI system consists of two main components:

1. **Voice AI UI (Frontend)**: A Next.js-based web application that provides a Spanish language user interface for interacting with the voice assistant. This interface is adaptable for web, kiosk ("Pop-Ups #YoSoyFuturo"), and mobile deployments.

2. **WebRTC Agent (Backend)**: A Python-based backend that handles speech processing, natural language understanding, and integration with government service knowledge bases.

The system leverages several key technologies:

- **WebRTC**: communication between frontend and backend
- **Text-to-Speech**: in Spanish with Dominican Spanish voice
- **Speech-to-Text**: optimized for Spanish language recognition
- **RAG System**: Retrieval-Augmented Generation for knowledge retrieval
- **Pattern Recognition**: Machine learning for anticipating citizen needs
- **Data Collection**: Secure storage of citizen interactions for service improvement

## Deployment Channels

TAINA is designed to be deployed across multiple channels:

1. **Physical Kiosks**: "Pop-Ups #YoSoyFuturo" located in high-traffic areas like shopping centers
2. **Web Platform**: Integration with the Gob.do platform
3. **Mobile App**: Integration with the Carpeta Ciudadana app
4. **Call Center**: Integration with government call center systems

## Government Service Integration

The system integrates with several government platforms:

- **GOB.DO**: Portal Único de Servicios del Gobierno Dominicano
- **Carpeta Ciudadana**: Citizen document management app
- **Call Center CRM**: Government call center knowledge base

## Testing Partnership

TAINA is being tested in collaboration with the Universidad del Caribe (UNICARIBE), where students provide valuable feedback on system performance, usability, and effectiveness in resolving citizen queries.

## Related Repositories

- [TAINA Voice AI UI (Frontend)]🔜
- [TAINA WebRTC Agent (Backend)]🔜

## Getting Started

To understand the system architecture, start with the [C4 Context Diagram](./2_Architecture/c4-model/2.1_Context_Diagram.md)🔜 which provides a high-level overview of the entire system and its interactions with government platforms and citizens.

For project management documentation, see the [Primary Use Cases](./3_Project_Management/use-cases/3.1_Primary_Use_Cases.md)🔜, [User Stories](./3_Project_Management/user-stories/)🔜, and the [Product Backlog](./3.8_Product_Backlog_TAINA.md)✅.

## Document Creation Timeline

- **Phase 1**: February 3-15, 2025 - Architecture Documentation
- **Phase 2**: February 17-28, 2025 - Project Management Documentation
- **Phase 3**: March 1-22, 2025 - Design, Testing, Data Collection, and Deployment Documentation
- **Review and Refinement**: March 24-April 20, 2025

## Contact Information

- **Project Manager**: [Name of PM](https://github.com)
- **Technical Writer**: [Name of TW](https://github.com)
- **Design Team**: [GeniaOps](https://github.com/GeniaOps)

## DISCLAIMER

### Concurrent Development and Documentation Activities
Our team initiated development of the "IA para la Ciudadanía" system without complete documentation or finalized architecture in order to meet aggressive delivery timelines. Documentation, architecture refinement, and development activities are now being conducted concurrently as the project progresses.
Our team continues to progress with development, architecture, and documentation based on preliminary timelines, but stakeholders should be aware that deliverable dates may require modification once official demonstration and launch dates are confirmed by the client.

### Timeline Uncertainty
Due to the absence of confirmed dates for system demonstration and official launch from the client, our project planning and resource allocation are subject to ongoing adjustments. This timeline uncertainty presents challenges for scheduling dependencies, coordinating with third-party partners (including UNICARIBE testing sessions), and establishing firm delivery milestones.

We remain committed to timely delivery while maintaining quality standards, and will promptly communicate any schedule adjustments as official dates are established.

