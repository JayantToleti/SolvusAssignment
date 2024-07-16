# SolvusAssignment
'''mermaid
graph TD
    User-->Chatbot
    Chatbot-->ChatbotController
    ChatbotController-->AuthService
    AuthService-->UserDatabase
    ChatbotController-->IntegrationLayer
    IntegrationLayer-->OCRService
    IntegrationLayer-->PrescriptionProcessor
    IntegrationLayer-->MedicineDatabaseService
    IntegrationLayer-->NotificationService
    OCRService-->PreprocessingModule
    OCRService-->RecognitionModule
    PreprocessingModule-->RecognitionModule
    RecognitionModule-->PrescriptionProcessor
    PrescriptionProcessor-->NLPModule
    NLPModule-->DataExtractor
    DataExtractor-->MedicineDatabaseService
    MedicineDatabaseService-->MedicineDatabase
    MedicineDatabaseService-->AlternativeMedicineService
    MedicineDatabaseService-->InventoryService
    MedicineDatabase-->MedicineDatabaseService
    AlternativeMedicineService-->MedicineDatabaseService
    InventoryService-->MedicineDatabaseService
    NotificationService-->EmailService
    NotificationService-->SMSServices
    IntegrationLayer-->AnalyticsService
    AnalyticsService-->LoggingService
    AnalyticsService-->MonitoringService
    IntegrationLayer-->ChatbotController
    ChatbotController-->Chatbot

''''
