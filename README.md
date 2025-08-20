# Automatic-Temperature-Controlled-System
This project simulates an automation system where a fan is automatically turned ON or OFF based on the room temperature.
#include <stdio.h>

int main() {
    float temperature;
    const float threshold = 30.0;  // Threshold temperature in Celsius

    printf("=== Automatic Temperature-Controlled Fan System ===\n");

    // Simulating continuous monitoring
    for (int i = 0; i < 5; i++) {  // Loop for 5 readings (can be extended)
        printf("\nEnter current room temperature (°C): ");
        scanf("%f", &temperature);

        if (temperature > threshold) {
            printf("🌡 Temperature = %.2f °C\n", temperature);
            printf("✅ Fan is AUTOMATICALLY TURNED ON.\n");
        } else {
            printf("🌡 Temperature = %.2f °C\n", temperature);
            printf("❌ Fan is AUTOMATICALLY TURNED OFF.\n");
        }
    }

    printf("\n--- Monitoring Completed ---\n");
    return 0;
}
