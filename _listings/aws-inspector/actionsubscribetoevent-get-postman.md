{
  "info": {
    "name": "AWS Inspector API Subscribe To Event",
    "_postman_id": "6ae4512c-c258-4d6e-96e4-c5c7c8d19e26",
    "description": "Enables the process of sending Amazon Simple Notification Service (SNS) notifications\n         about a specified event to a specified SNS topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "e2157fa4-3b2e-4d73-a4fa-5ba22c64efff",
          "name": "addAttributesToFindings",
          "request": {
            "url": "http://example.com/api/?Action=AddAttributesToFindings?attributes=attributes&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns attributes (key and value pairs) to the findings that are specified by the\n         ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21a3b5db-5235-417d-836b-e93e43996c1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Targets",
      "item": [
        {
          "id": "e71d9cc1-ee56-4776-ae7b-a679cd757a4d",
          "name": "createAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTarget?assessmentTargetName=assessmentTargetName&resourceGroupArn=resourceGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new assessment target using the ARN of the resource group that is generated\n         by."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "567aff29-0baf-4e9b-be93-e3b98e853d90"
            }
          ]
        },
        {
          "id": "55e66a47-a664-44ef-b276-87485fb44326",
          "name": "deleteAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTarget?assessmentTargetArn=assessmentTargetArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment target that is specified by the ARN of the assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce3bf18e-96c6-4900-bfe6-d9fc41da82cf"
            }
          ]
        },
        {
          "id": "d1adc99b-d099-4af9-9a45-999a6bda5a04",
          "name": "describeAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTargets?assessmentTargetArns=assessmentTargetArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment targets that are specified by the ARNs of the assessment\n         targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85cb87e5-9d1c-473b-9ce2-ee4eddc24e8f"
            }
          ]
        },
        {
          "id": "ee3c0d72-ce56-4205-b21d-c0ce742c16ba",
          "name": "listAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTargets?filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the ARNs of the assessment targets within this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4c4712e-8307-4752-9d07-9cc91fa396b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Templates",
      "item": [
        {
          "id": "d60f143f-4a35-482c-a9ed-c6e54ca0abc0",
          "name": "createAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTemplate?assessmentTargetArn=assessmentTargetArn&assessmentTemplateName=assessmentTemplateName&durationInSeconds=durationInSeconds&rulesPackageArns=rulesPackageArns&userAttributesForFindings=userAttributesForFindings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an assessment template for the assessment target that is specified by the ARN\n         of the assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "487ee911-7cd5-4303-bc5a-7a9089bd76c6"
            }
          ]
        },
        {
          "id": "451404b0-e8b3-47ac-9b5e-059a434efa9d",
          "name": "deleteAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTemplate?assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment template that is specified by the ARN of the assessment\n         template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf7b7c90-009b-4b16-8547-bd127266bce5"
            }
          ]
        },
        {
          "id": "9b6ca331-831c-4ac0-9b29-4504d27e65f6",
          "name": "describeAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTemplates?assessmentTemplateArns=assessmentTemplateArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment templates that are specified by the ARNs of the assessment\n         templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f50701b-b1ef-44fe-ae1f-a19c00674be5"
            }
          ]
        },
        {
          "id": "7ca889bb-9936-439c-b22b-55c0fc2eddea",
          "name": "listAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTemplates?assessmentTargetArns=assessmentTargetArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment templates that correspond to the assessment targets that are\n         specified by the ARNs of the assessment targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b436693-9967-42bc-8be1-183fcb358c94"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Groups",
      "item": [
        {
          "id": "c9c53aff-8c9b-4532-b9b1-5318464aa0ee",
          "name": "createResourceGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateResourceGroup?resourceGroupTags=resourceGroupTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a resource group using the specified set of tags (key and value pairs) that\n         are used to select the EC2 instances to be included in an Amazon Inspector assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63dc723b-cc01-468e-bdf9-da106eb032bb"
            }
          ]
        },
        {
          "id": "4d979dea-2368-4628-8f90-92c386aa0322",
          "name": "describeResourceGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeResourceGroups?resourceGroupArns=resourceGroupArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the resource groups that are specified by the ARNs of the resource\n         groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af512dc3-3635-48d1-9f0e-d46ff7cfef48"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Runs",
      "item": [
        {
          "id": "04a44efe-af9f-4d44-ae22-786a234f362c",
          "name": "deleteAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6107a984-2479-47e5-9dd0-8e656a2dcec5"
            }
          ]
        },
        {
          "id": "88657b7a-0261-46d3-ba45-39fb297f8eb2",
          "name": "describeAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentRuns?assessmentRunArns=assessmentRunArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment runs that are specified by the ARNs of the assessment\n         runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "317cda01-3b1d-4625-b360-2f065df0cde7"
            }
          ]
        },
        {
          "id": "cb7e5a3e-4880-4bae-88ef-d540cd420839",
          "name": "listAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRuns?assessmentTemplateArns=assessmentTemplateArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment runs that correspond to the assessment templates that are\n         specified by the ARNs of the assessment templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4484ed6e-a053-4c10-91f8-13d76939483b"
            }
          ]
        },
        {
          "id": "59aeffb7-758f-4a39-8dc2-cc0a3cedb624",
          "name": "startAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StartAssessmentRun?assessmentRunName=assessmentRunName&assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the assessment run specified by the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12a432e9-1a5f-4c17-9f1c-e7ada6a24522"
            }
          ]
        },
        {
          "id": "2f8ffcf2-396f-4f16-ae63-ed75e8d31c35",
          "name": "stopAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StopAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f12cc459-7b95-493b-a7e3-7dd247e3fc10"
            }
          ]
        }
      ]
    },
    {
      "name": "Cross Account Access Roles",
      "item": [
        {
          "id": "845bba95-c44e-4776-a6ab-4f4a9012808d",
          "name": "describeCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCrossAccountAccessRole?registeredAt=registeredAt&roleArn=roleArn&valid=valid",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the IAM role that enables Amazon Inspector to access your AWS\n         account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c5a0532-b080-4794-ba0c-83a0f4b83d39"
            }
          ]
        },
        {
          "id": "1246d328-7dd0-4b50-add2-03d6072635e1",
          "name": "registerCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=RegisterCrossAccountAccessRole?roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers the IAM role that Amazon Inspector uses to list your EC2 instances at the\n         start of the assessment run or when you call the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c32af55-ae2c-4aad-85f5-3f36e0c69820"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "e81b8e6a-871f-4507-8d30-f4a3b1282fca",
          "name": "describeFindings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFindings?findingArns=findingArns&locale=locale",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the findings that are specified by the ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a212e175-9a1b-4480-bebc-ed7bdd232996"
            }
          ]
        },
        {
          "id": "d8bb89a0-3d0c-4b3a-a2b8-5151e1008a58",
          "name": "listFindings",
          "request": {
            "url": "http://example.com/api/?Action=ListFindings?assessmentRunArns=assessmentRunArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists findings that are generated by the assessment runs that are specified by the\n         ARNs of the assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5ec1f94-adbb-4e13-a468-0ba633c9637d"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules Packages",
      "item": [
        {
          "id": "ef7f4a60-7892-4cd9-8c18-3a6d6240a7cf",
          "name": "describeRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRulesPackages?locale=locale&rulesPackageArns=rulesPackageArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the rules packages that are specified by the ARNs of the rules\n         packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "888fb620-6329-4602-b791-56c8cc20121d"
            }
          ]
        },
        {
          "id": "126d1c14-c6f3-407f-8f53-ac5afbe41951",
          "name": "listRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=ListRulesPackages?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all available Amazon Inspector rules packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "251a4f58-42e3-4f10-bef0-b04835bedfd2"
            }
          ]
        }
      ]
    },
    {
      "name": "Telemetry Metadata",
      "item": [
        {
          "id": "edd6f05f-b4ed-49a6-9a8f-2161de294274",
          "name": "getTelemetryMetadata",
          "request": {
            "url": "http://example.com/api/?Action=GetTelemetryMetadata?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the data that is collected for the specified assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "882efa73-cde8-463a-872e-2478de75d11b"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Run Agents",
      "item": [
        {
          "id": "a5947ec9-acee-4979-b40f-3a254fb37f2c",
          "name": "listAssessmentRunAgents",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRunAgents?assessmentRunArn=assessmentRunArn&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the agents of the assessment runs that are specified by the ARNs of the\n         assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7c481ab-b52c-49c0-83f9-49564953d341"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "afaf53e1-dadb-47ea-be9c-9f687b700c97",
          "name": "listEventSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListEventSubscriptions?maxResults=maxResults&nextToken=nextToken&resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the event subscriptions for the assessment template that is specified by\n         the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87f5d068-1173-4baa-831f-7475f88d7b63"
            }
          ]
        },
        {
          "id": "ac8ec41c-8086-4e0d-bc4d-84ff994a5633",
          "name": "subscribeToEvent",
          "request": {
            "url": "http://example.com/api/?Action=SubscribeToEvent?event=event&resourceArn=resourceArn&topicArn=topicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the process of sending Amazon Simple Notification Service (SNS) notifications\n         about a specified event to a specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f2be2f3-fe0d-4ebc-aa0f-312ee2bcf877"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags For Resources",
      "item": [
        {
          "id": "ada96b72-472f-4776-8f67-d85f58c04ea0",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags associated with an assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "459b52ef-01a6-4a77-8b3b-01d874fa2d0f"
            }
          ]
        },
        {
          "id": "984e8db9-d40a-43ba-9f41-6a71c0856ed6",
          "name": "setTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=SetTagsForResource?resourceArn=resourceArn&tags=tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets tags (key and value pairs) to the assessment template that is specified by the\n         ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "869c705a-7d84-4574-adaa-cdb8e5df1cfa"
            }
          ]
        }
      ]
    },
    {
      "name": "Agents",
      "item": [
        {
          "id": "3ddc7c33-f521-484c-8990-98a91dff4b20",
          "name": "previewAgents",
          "request": {
            "url": "http://example.com/api/?Action=PreviewAgents?maxResults=maxResults&nextToken=nextToken&previewAgentsArn=previewAgentsArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Previews the agents installed on the EC2 instances that are part of the specified\n         assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30fa3d50-b2ba-44a3-9375-86b4c6ba090d"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes From Findings",
      "item": [
        {
          "id": "ebb30045-049a-4e42-956e-3ef0d800531d",
          "name": "removeAttributesFromFindings",
          "request": {
            "url": "http://example.com/api/?Action=RemoveAttributesFromFindings?attributeKeys=attributeKeys&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes entire attributes (key and value pairs) from the findings that are specified\n         by the ARNs of the findings where an attribute with the specified key exists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10f71cfa-6972-4d90-917d-afd2658f234e"
            }
          ]
        }
      ]
    }
  ]
}