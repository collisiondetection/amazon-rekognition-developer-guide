# TextDetection<a name="API_TextDetection"></a>

Information about a word or line of text detected by [DetectText](API_DetectText.md)\.

The `DetectedText` field contains the text that Amazon Rekognition detected in the image\. 

Every word and line has an identifier \(`Id`\)\. Each word belongs to a line and has a parent identifier \(`ParentId`\) that identifies the line of text in which the word appears\. The word `Id` is also an index for the word within a line of words\. 

For more information, see [Detecting Text](text-detection.md)\.

## Contents<a name="API_TextDetection_Contents"></a>

 **Confidence**   
The confidence that Amazon Rekognition has in the accuracy of the detected text and the accuracy of the geometry points around the detected text\.  
Type: Float  
Valid Range: Minimum value of 0\. Maximum value of 100\.  
Required: No

 **DetectedText**   
The word or line of text recognized by Amazon Rekognition\.   
Type: String  
Required: No

 **Geometry**   
The location of the detected text on the image\. Includes an axis aligned coarse bounding box surrounding the text and a finer grain polygon for more accurate spatial information\.  
Type: [Geometry](API_Geometry.md) object  
Required: No

 **Id**   
The identifier for the detected text\. The identifier is only unique for a single call to `DetectText`\.   
Type: Integer  
Valid Range: Minimum value of 0\.  
Required: No

 **ParentId**   
The Parent identifier for the detected text identified by the value of `ID`\. If the type of detected text is `LINE`, the value of `ParentId` is `Null`\.   
Type: Integer  
Valid Range: Minimum value of 0\.  
Required: No

 **Type**   
The type of text that was detected\.  
Type: String  
Valid Values:` LINE | WORD`   
Required: No

## See Also<a name="API_TextDetection_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:

+  [AWS SDK for C\+\+](http://docs.aws.amazon.com/goto/SdkForCpp/rekognition-2016-06-27/TextDetection) 

+  [AWS SDK for Go](http://docs.aws.amazon.com/goto/SdkForGoV1/rekognition-2016-06-27/TextDetection) 

+  [AWS SDK for Java](http://docs.aws.amazon.com/goto/SdkForJava/rekognition-2016-06-27/TextDetection) 

+  [AWS SDK for Ruby V2](http://docs.aws.amazon.com/goto/SdkForRubyV2/rekognition-2016-06-27/TextDetection) 