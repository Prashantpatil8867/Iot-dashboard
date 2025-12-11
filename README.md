# IoT-based Weather Monitoring System

A comprehensive IoT weather monitoring solution featuring ESP32-based sensor nodes, Spring Boot REST API, and web-based dashboard for real-time weather data collection and visualization.

## 🌟 Features

- **IoT Sensor Nodes**: ESP32-based weather stations for data collection
- **REST API**: Spring Boot backend for data management and processing
- **Web Dashboard**: Real-time weather data visualization
- **Database Integration**: PostgreSQL for reliable data storage
- **Circuit Design**: Custom PCB fabrication files included
- **Scalable Architecture**: Support for multiple weather monitoring nodes

## 🏗️ Project Structure

```
IoT-based-Weather-Monitoring-System/
├── Weather-API/                    # Spring Boot REST API
│   ├── src/main/java/             # Java source code
│   ├── src/main/resources/        # Configuration files
│   └── pom.xml                    # Maven dependencies
├── weatherNodeFirmware/           # ESP32 firmware code
├── adminDashboard/               # Web dashboard application
├── circuitAndPCBFabricationFiles/ # Hardware design files
└── readme.md                     # Project documentation
```

## 🛠️ Technology Stack

### Backend
- **Spring Boot 2.7.2** - REST API framework
- **Java 18** - Programming language
- **Spring Data JPA** - Database abstraction
- **PostgreSQL** - Primary database
- **Maven** - Dependency management

### Hardware
- **ESP32** - Microcontroller for sensor nodes
- **Custom PCB** - Weather sensor integration

### Frontend
- **Web Dashboard** - Real-time data visualization
- **Admin Panel** - System management interface

## 🚀 Getting Started

### Prerequisites

- Java 18 or higher
- Maven 3.6+
- PostgreSQL database
- ESP32 development environment
- Git

### API Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd IoT-based-Weather-Monitoring-System-main
   ```

2. **Configure Database**
   - Install PostgreSQL
   - Create a database for the weather system
   - Update `application.properties` with your database credentials

3. **Build and Run API**
   ```bash
   cd Weather-API
   ./mvnw clean install
   ./mvnw spring-boot:run
   ```

### Hardware Setup

1. **ESP32 Configuration**
   - Flash the firmware from `weatherNodeFirmware/` directory
   - Configure WiFi credentials and API endpoints
   - Connect weather sensors according to circuit diagrams

2. **PCB Fabrication** (Optional)
   - Use files in `circuitAndPCBFabricationFiles/` for custom PCB manufacturing
   - Follow assembly instructions for sensor integration

## 📡 API Endpoints

The Spring Boot API provides endpoints for:
- Weather data ingestion from IoT nodes
- Historical data retrieval
- Node management and configuration
- Real-time data streaming

## 🔧 Configuration

### Database Configuration
Update `Weather-API/src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/weather_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### ESP32 Configuration
Configure your ESP32 nodes with:
- WiFi network credentials
- API server endpoint
- Sensor calibration parameters

## 📊 Dashboard

Access the web dashboard for:
- Real-time weather data visualization
- Historical trend analysis
- Node status monitoring
- System administration

**Live Demo**: https://admindash-017.herokuapp.com/

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 Development Status

> **Notice**: This project is undergoing a complete revamp with new features. For viewing older code, please switch to the `legacy` branch.

### Current Version Features:
- ✅ Spring Boot REST API
- ✅ PostgreSQL integration
- ✅ ESP32 firmware foundation
- 🚧 Web dashboard (in development)
- 🚧 Enhanced sensor support
- 🚧 Real-time notifications

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support and questions:
- Create an issue in the GitHub repository
- Check the documentation in each component directory
- Review the legacy branch for reference implementations

## 🔮 Roadmap

- [ ] Enhanced web dashboard with charts and analytics
- [ ] Mobile application support
- [ ] Advanced weather prediction algorithms
- [ ] Multi-location monitoring support
- [ ] Cloud deployment automation
- [ ] Enhanced security features
