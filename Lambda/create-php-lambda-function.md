# Create a Lambda PHP Function

1. Author function from Scratch & select "Use custom runtime in function code or layer"
1. Click Layers & add new layer
1. Add Layer from ARN `arn:aws:lambda:<region>:887080169480:layer:php71:6` - Check https://github.com/stackery/php-lambda-layer for latest version.
1. Save function.
1. Click on the function name (above Layers)
1. Upload zip with index.php 
1. Update your handler to be index.php
1. Add API Gateway Trigger
1. Fill in the API Gateway details
1. Save Function
1. Test lambda function by hitting API Gateway endpoint

# FAQs

How do you enable extensions?
 - Create a `php.ini` in the project root and add the extensions (e.g `extension=xml.so`)