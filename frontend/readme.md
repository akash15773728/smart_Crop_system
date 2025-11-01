<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AgriPredict - Barebones Prototype</title>
</head>
<body style="font-family: sans-serif; margin: 20px; background-color: #f0f0f0;">

    <!-- Header -->
    <h1 style="text-align: center;">AgriPredict</h1>
    <p style="text-align: center; color: #555;">Choose a link.</p>
    <hr>

    <!-- Main Content Area -->
    <div id="feature-container" style="max-width: 800px; margin: 20px auto;">
        
        <!-- Features -->

        <!-- 1. Crop Recommendation Card -->
        <div id="crop" style="border: 1px solid #ccc; padding: 10px; margin-bottom: 10px; background-color: white;">
            <p><strong>Crop Recommendation</strong></p>
            <p style="font-size: 12px; color: #777;">Inputs: Soil data, Season, Location</p>
            <a href="#crop-detail" onclick="startFeature('crop')">Start Feature →</a>
        </div>

        <!-- 2. Fertilizer Guidance Card -->
        <div id="fertilizer" style="border: 1px solid #ccc; padding: 10px; margin-bottom: 10px; background-color: white;">
            <p><strong>Fertilizer Guidance</strong></p>
            <p style="font-size: 12px; color: #777;">Inputs: Soil Test Report, Crop Type</p>
            <a href="#fertilizer-detail" onclick="startFeature('fertilizer')">Start Feature →</a>
        </div>

        <!-- 3. Weather Alerts Card -->
        <div id="weather" style="border: 1px solid #ccc; padding: 10px; margin-bottom: 10px; background-color: white;">
            <p><strong>Weather Alerts</strong></p>
            <p style="font-size: 12px; color: #777;">Outputs: Real-time temperature & rainfall</p>
            <a href="#weather-detail" onclick="startFeature('weather')">Start Feature →</a>
        </div>

        <!-- 4. Pest Detection Card -->
        <div id="pest" style="border: 1px solid #ccc; padding: 10px; margin-bottom: 10px; background-color: white;">
            <p><strong>Pest Detection</strong></p>
            <p style="font-size: 12px; color: #777;">Inputs: Image upload/camera, Crop health</p>
            <a href="#pest-detail" onclick="startFeature('pest')">Start Feature →</a>
        </div>

        <!-- 5. Market Prices Card -->
        <div id="market" style="border: 1px solid #ccc; padding: 10px; margin-bottom: 10px; background-color: white;">
            <p><strong>Market Prices</strong></p>
            <p style="font-size: 12px; color: #777;">Outputs: Commodity prices, trend data</p>
            <a href="#market-detail" onclick="startFeature('market')">Start Feature →</a>
        </div>

        <!-- 6. Voice Support Card -->
        <div id="voice" style="border: 1px solid #ccc; padding: 10px; margin-bottom: 10px; background-color: white;">
            <p><strong> Voice Support</strong></p>
            <p style="font-size: 12px; color: #777;">Inputs: Local language spoken query</p>
            <a href="#voice-detail" onclick="startFeature('voice')">Start Feature →</a>
        </div>
    </div>
    
    <hr>
    
    <!--JavaScript Logic -->
    <script>
    

        // Function to handle feature navigation (now uses onclick for simplicity)
        function startFeature(featureId) {
            console.log([WIP] Feature selected: ${featureId}. Logic needs to be written here.);
            alert(Opening ${featureId.toUpperCase()} Feature... (TODO: Implement UI here)); 
            // Note: In a real hackathon, we would use a proper modal instead of alert()!
        }

        // Placeholder for future API integration
        function futureApiCall(endpoint) {
            console.log([TODO] Connect to backend API endpoint: /api/${endpoint});
            // return fetch(/api/${endpoint});
        }

        // Main app initialization (barely started)
        document.addEventListener('DOMContentLoaded', () => {
            console.log("AgriPredict minimal script started.");
            // futureApiCall('initial-data-load');
        });

    </script>
</body>
</html>
