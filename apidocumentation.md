---
layout: tailwind
search_exclude: true
hide: true
show_reading_time: false
permalink: /apidocumentation
---

<div class="space-y-8">
  <section class="bg-dark rounded-lg p-8 shadow-lg">
    <h1 class="text-4xl font-bold text-accent mb-4">CrossWise API Documentation</h1>
    <h2 class="text-2xl text-gray-300 mb-6">Technical Implementation Overview</h2>
    
    <p class="text-gray-200 mb-6">
      This documentation outlines the major technical accomplishments and API components that power the CrossWise Smart Guide application. Our system combines real-time data scraping, machine learning forecasting, and social media monitoring to provide accurate border crossing predictions.
    </p>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="table-of-contents">
    <h2 class="text-2xl font-bold text-accent mb-4">API Components Overview</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
      <a href="#prediction-api" class="text-gray-200 hover:text-accent">1. Intelligent Wait Time Prediction API</a>
      <a href="#visualization-api" class="text-gray-200 hover:text-accent">2. Historical Visualization API</a>
      <a href="#social-monitoring" class="text-gray-200 hover:text-accent">3. Live Social Media Monitoring</a>
      <a href="#facial-recognition" class="text-gray-200 hover:text-accent">4. Facial Recognition Utility</a>
      <a href="#weather-helper" class="text-gray-200 hover:text-accent">5. Weather Normalization Helper</a>
      <a href="#timelapse-generator" class="text-gray-200 hover:text-accent">6. Timelapse Video Generator</a>
      <a href="#feedback-collector" class="text-gray-200 hover:text-accent">7. Border Feedback Collector</a>
      <a href="#video-crawler" class="text-gray-200 hover:text-accent">8. Automated Border Video Crawler</a>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="prediction-api">
    <h2 class="text-2xl font-bold text-accent mb-4">1. Intelligent Wait Time Prediction API</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: border.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Designed a smart prediction API that uses both real-time scraping and ML-based long-term forecasting to return expected border wait times.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Provides highly relevant, accurate crossing time estimates for users planning trips.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Dual-mode support for both <code class="bg-gray-800 px-2 py-1 rounded">long_term</code> and <code class="bg-gray-800 px-2 py-1 rounded">today</code> predictions</li>
          <li>Dynamic handling of missing inputs (<code class="bg-gray-800 px-2 py-1 rounded">month</code>, <code class="bg-gray-800 px-2 py-1 rounded">day</code>, <code class="bg-gray-800 px-2 py-1 rounded">hour</code>) using <code class="bg-gray-800 px-2 py-1 rounded">datetime</code></li>
          <li>Custom weighted average algorithm that compares CBP real-time data to historical averages</li>
          <li>Intelligent fallback mechanisms for data unavailability scenarios</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="visualization-api">
    <h2 class="text-2xl font-bold text-accent mb-4">2. Historical Visualization API with Plotly</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: historicalgraph_api.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Built a visual API endpoint that returns an interactive Plotly chart displaying average hourly wait times across weekdays.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Helps users and analysts find patterns in border congestion throughout the week.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Clean mapping of JSON data to pandas DataFrame for efficient processing</li>
          <li>Interactive Plotly visualizations with hover templates, line graphs, and annotations</li>
          <li>Advanced color coding and hover cues to focus on congestion trends</li>
          <li>Seamless HTML output via Flask <code class="bg-gray-800 px-2 py-1 rounded">Response</code> object</li>
          <li>Responsive design that adapts to different screen sizes</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="social-monitoring">
    <h2 class="text-2xl font-bold text-accent mb-4">3. Live Social Media Monitoring</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">Files: twitter.py, twitter_search.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Implemented a Twitter-based keyword listener that extracts tweets about border delays and incidents.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Augments our data model with real user reports on unusual delays, accidents, or alerts from the border community.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Sophisticated query construction using geotagged search for the border region</li>
          <li>Secure integration with Twitter Bearer Token authentication</li>
          <li>Pluggable architecture via <code class="bg-gray-800 px-2 py-1 rounded">run_border_queries()</code> in main runtime</li>
          <li>Real-time sentiment analysis and keyword filtering</li>
          <li>Automated anomaly detection for unusual border events</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="facial-recognition">
    <h2 class="text-2xl font-bold text-accent mb-4">4. Facial Recognition Encoding Utility</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: facial_encoding.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Built a utility using the <code class="bg-gray-800 px-2 py-1 rounded">face_recognition</code> library to generate secure encodings from user-submitted images.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Enables future authentication or personalization features while maintaining user privacy and security.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Advanced face landmark detection and feature extraction</li>
          <li>Secure encoding storage in a consistent, encrypted format</li>
          <li>Modular utility design for easy expansion and integration</li>
          <li>Privacy-first approach with no raw image storage</li>
          <li>Error handling for various image formats and quality levels</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="weather-helper">
    <h2 class="text-2xl font-bold text-accent mb-4">5. Weather Normalization Helper</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: weather_formater.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Converts raw weather data into structured summaries with icons and descriptive text.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Supports context-aware guidance such as "Expect longer delays during fog" or "Clear weather - normal wait times expected."
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Comprehensive mapping of weather codes to descriptive conditions</li>
          <li>Clean separation of formatting logic for optimized API consumption</li>
          <li>Multi-language support for weather descriptions</li>
          <li>Integration with border wait time correlation algorithms</li>
          <li>Automated weather impact assessment on crossing conditions</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="timelapse-generator">
    <h2 class="text-2xl font-bold text-accent mb-4">6. Timelapse Video Generator (Traffic Review)</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: timelapse.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Generated stitched video summaries using saved traffic cam footage throughout a day.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Allows users to visually review congestion patterns before choosing optimal crossing times.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Efficient use of <code class="bg-gray-800 px-2 py-1 rounded">moviepy</code> for MP4 composition and rendering</li>
          <li>Organized file structure with timestamped folders for easy navigation</li>
          <li>Automated video quality optimization for web delivery</li>
          <li>Customizable playback speeds and time intervals</li>
          <li>Integration with historical wait time data overlay</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="feedback-collector">
    <h2 class="text-2xl font-bold text-accent mb-4">7. Structured Border Feedback Collector</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: border_feedback.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Created a comprehensive feedback API to gather user reports on real-life wait experiences.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Trains and improves our long-term prediction models using community-submitted data and real user experiences.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Robust validation for email, rating, and location fields</li>
          <li>Automated timestamp generation and secure data storage</li>
          <li>Integration with machine learning training pipelines</li>
          <li>Anonymous feedback options for privacy-conscious users</li>
          <li>Real-time feedback analysis for immediate system improvements</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="video-crawler">
    <h2 class="text-2xl font-bold text-accent mb-4">8. Automated Border Video Crawler</h2>
    
    <div class="bg-darker rounded-lg p-6 mb-6">
      <h3 class="text-xl font-semibold text-success mb-3">File: video_crawler.py</h3>
      
      <p class="text-gray-200 mb-4">
        <strong>Accomplishment:</strong> Developed a sophisticated background script that crawls and downloads time-stamped traffic cam footage from the San Ysidro crossing every 29 seconds.
      </p>
      
      <p class="text-gray-200 mb-4">
        <strong>Purpose:</strong> Supports timelapse generation and historical visual analysis of real border wait conditions throughout the day.
      </p>
      
      <div>
        <h4 class="text-lg font-semibold text-gray-100 mb-3">Key Highlights:</h4>
        <ul class="list-disc pl-5 space-y-2 text-gray-200">
          <li>Automated pulling of <code class="bg-gray-800 px-2 py-1 rounded">.mp4</code> clips from <code class="bg-gray-800 px-2 py-1 rounded">bordertraffic.com</code> based on UTC-formatted filenames</li>
          <li>Advanced use of <code class="bg-gray-800 px-2 py-1 rounded">pytz</code> to localize timestamps to Pacific Time</li>
          <li>Intelligent backfill logic to download the past 2 hours of footage if no files exist on launch</li>
          <li>Comprehensive error handling for unavailable videos and server timeouts</li>
          <li>Retry mechanisms with exponential backoff for network resilience</li>
          <li>Efficient storage management with automatic cleanup of old footage</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg" id="system-overview">
    <h2 class="text-2xl font-bold text-accent mb-4">System Architecture Overview</h2>
    
    <p class="text-gray-200 mb-6">
      Together, these components demonstrate a comprehensive approach to border crossing prediction and management:
    </p>
    
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">Full-Stack Engineering</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>RESTful APIs with comprehensive documentation</li>
          <li>Advanced data models and database optimization</li>
          <li>Interactive visualization components</li>
          <li>Utility scripts for automation and maintenance</li>
        </ul>
      </div>
      
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">ML + Real-time Forecasting</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>Machine learning algorithms for pattern recognition</li>
          <li>Real-time data integration and processing</li>
          <li>Predictive modeling with continuous improvement</li>
          <li>Multi-source data fusion for accuracy</li>
        </ul>
      </div>
      
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">Usability and Reliability</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>User-centered design principles</li>
          <li>Robust error handling and fallback mechanisms</li>
          <li>Performance optimization and caching strategies</li>
          <li>Comprehensive testing and monitoring</li>
        </ul>
      </div>
      
      <div class="bg-darker rounded-lg p-6">
        <h3 class="text-xl font-semibold text-success mb-3">Scalability and Security</h3>
        <ul class="list-disc pl-5 space-y-1 text-gray-200">
          <li>Modular architecture for easy expansion</li>
          <li>Secure data handling and privacy protection</li>
          <li>API rate limiting and authentication</li>
          <li>Cloud-ready deployment strategies</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="bg-dark rounded-lg p-8 shadow-lg">
    <div class="mt-8 p-4 border border-gray-700 rounded-md text-center">
      <p class="text-gray-300">
        This API documentation represents the technical foundation of CrossWise Smart Guide's intelligent border crossing prediction system. Each component is designed for reliability, scalability, and continuous improvement.
      </p>
      <p class="text-gray-400 mt-4 text-sm italic">
        For technical support or integration questions, please contact our development team. All APIs include comprehensive error handling and detailed logging for debugging and monitoring purposes.
      </p>
    </div>
  </section>
</div>
