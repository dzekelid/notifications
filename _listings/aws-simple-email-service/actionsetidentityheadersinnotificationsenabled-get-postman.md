{
  "info": {
    "name": "AWS Simple Email Service API Set Identity Headers In Notifications Enabled",
    "_postman_id": "4da236e6-9f47-4d7a-ac7d-cc06da4e30eb",
    "description": "Given an identity (an email address or a domain), sets whether Amazon SES includes \n            the original email headers in the Amazon Simple Notification Service (Amazon SNS) notifications \n            of a specified type.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "13b4c514-056a-4901-9b19-6595b8489126",
          "name": "cloneReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CloneReceiptRuleSet?OriginalRuleSetName=OriginalRuleSetName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule set by cloning an existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1a80906-344f-428d-8fad-06f71a664287"
            }
          ]
        },
        {
          "id": "f0b7bfb5-0d14-4e0b-8aa9-fa54d0b3a263",
          "name": "createReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b93016c-f3da-459b-b26c-69e349d83175"
            }
          ]
        },
        {
          "id": "4aedc71e-022b-424a-8699-55d71fd9e9f7",
          "name": "deleteReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule set and all of the receipt rules it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6df43790-8e60-4534-8ff2-578163d923db"
            }
          ]
        },
        {
          "id": "ca34d3e0-bfb9-4951-9f97-ee3123b39813",
          "name": "describeActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActiveReceiptRuleSet?Metadata=Metadata&Rules.member.N=Rules.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03cd5c30-0201-4090-933b-90f777e89a35"
            }
          ]
        },
        {
          "id": "ad607bb5-542e-46a6-bc87-58600f620625",
          "name": "describeReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bdaf5cf-3548-4a94-8d9d-1257916cd96b"
            }
          ]
        },
        {
          "id": "ceb14816-f142-4356-bbe2-14c4b848345a",
          "name": "listReceiptRuleSets",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptRuleSets?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the receipt rule sets that exist under your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00cf76d5-b25e-423f-ae8b-b31170e66d5b"
            }
          ]
        },
        {
          "id": "211c148d-5a0f-433c-b85a-1bdca4e5ef8e",
          "name": "reorderReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=ReorderReceiptRuleSet?RuleNames.member.N=RuleNames.member.N&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reorders the receipt rules within a receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7f552e8-68b1-405f-a165-b831e86fa68f"
            }
          ]
        },
        {
          "id": "afd684db-2454-468f-8140-486bd0a4a0b9",
          "name": "setActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=SetActiveReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the specified receipt rule set as the active receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6fde3a7-1422-4235-80a4-53c5a546be45"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "c7aba9b8-cddb-4739-a90b-a48e159b11ca",
          "name": "createConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSet?ConfigurationSet=ConfigurationSet",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db53577f-0a2b-4432-8ae5-9529d2032247"
            }
          ]
        },
        {
          "id": "bdafc2a3-d6fe-4871-8488-b53ee4cda666",
          "name": "deleteConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSet?ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "896aec58-55c5-4384-8e92-c155902c237b"
            }
          ]
        },
        {
          "id": "21ecd6b4-f08c-4c2e-9b2e-7ea902a68a06",
          "name": "describeConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSet?ConfigurationSetAttributeNames.member.N=ConfigurationSetAttributeNames.member.N&ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "449ee1ad-8c3b-441a-91f3-149fa4894603"
            }
          ]
        },
        {
          "id": "42efc66c-8569-49df-b563-ce0202ec2465",
          "name": "listConfigurationSets",
          "request": {
            "url": "http://example.com/api/?Action=ListConfigurationSets?MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the configuration sets associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abc4b40f-4aae-496b-afc7-b7d507cc0bcf"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "8bcf4b71-4ecf-4882-9309-3f3055419226",
          "name": "createConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55d544d7-7a55-4085-ac30-84c3b4986444"
            }
          ]
        },
        {
          "id": "7727df37-763d-4d2f-b815-eaffc9e21bf4",
          "name": "deleteConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestinationName=EventDestinationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95d22d22-b127-40c3-843f-6b52c0e86b22"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "e3a8e5e4-07e2-4a2e-beef-a9b4208d00d9",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4aca34e8-10ed-4407-ba5b-df138a53d2d9"
            }
          ]
        },
        {
          "id": "8111dde6-850f-4c47-8ab1-e9104b80e24c",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f1f01da-eab2-484b-b6c1-4a31939c370f"
            }
          ]
        },
        {
          "id": "018afc96-5c19-4384-a993-395575fa3b64",
          "name": "listReceiptFilters",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptFilters?Filters.member.N=Filters.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IP address filters associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78f8e317-43ef-4a52-8652-2c24911d2ba0"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "19803139-9152-4345-9e35-c190d5475792",
          "name": "createReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRule?After=After&Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d335e53-8db1-49ad-80aa-7406c68cb889"
            }
          ]
        },
        {
          "id": "7db0f8e2-5be4-495e-9c22-bbec251144a4",
          "name": "deleteReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5160fb-4361-465d-9f58-ef3ec6e4cf42"
            }
          ]
        },
        {
          "id": "d500404f-33db-4b2f-9b8f-cc6c9a0cc013",
          "name": "describeReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56bd1fce-989f-41ef-b7da-21a39ab5e14b"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "1e18ab97-5db3-434c-b440-a25b8b2c3f9e",
          "name": "deleteIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentity?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified identity (an email address or a domain) from the list of verified identities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6dd8b88-89d1-4424-991e-aa3816010dc2"
            }
          ]
        },
        {
          "id": "47614d65-14c7-4aaf-a98c-2d7ec59958fe",
          "name": "deleteIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPolicy?Identity=Identity&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified sending authorization policy for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b7d1c38-e0b6-4982-b6d1-b583346a486e"
            }
          ]
        },
        {
          "id": "a6961859-76f9-4269-89a8-ce33f5260605",
          "name": "getIdentityDkimAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityDkimAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current status of Easy DKIM signing for an entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c46848d-cd2c-43fd-ab6a-27826f25eeb6"
            }
          ]
        },
        {
          "id": "83dcb9cf-4f07-4119-be30-7678fd04ada4",
          "name": "getIdentityMailFromDomainAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityMailFromDomainAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the custom MAIL FROM attributes for a list of identities (email addresses and/or domains)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb4f00a9-368f-45b3-8748-cb3cb1178b23"
            }
          ]
        },
        {
          "id": "54e1dd93-510a-4120-89f4-cd6784eca9c4",
          "name": "getIdentityNotificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityNotificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of verified identities (email addresses and/or domains), returns a structure describing identity notification attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68ac8ccc-5962-401a-9e74-2c41f75c3e67"
            }
          ]
        },
        {
          "id": "b9299488-deb2-4429-a379-7a8a531bda40",
          "name": "getIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPolicies?Identity=Identity&PolicyNames.member.N=PolicyNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a8178e4-9df9-441f-9ab6-4b75ab8c0af6"
            }
          ]
        },
        {
          "id": "44b0f237-f175-4b46-9a2a-f0786fb5a13c",
          "name": "getIdentityVerificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityVerificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of identities (email addresses and/or domains), returns the verification status and (for domain identities) the verification token for each identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d91b54d-c1e3-4102-85ce-5adda10f8554"
            }
          ]
        },
        {
          "id": "6eaf49b4-66f3-44a2-85cd-aab2c8483179",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?IdentityType=IdentityType&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9357a68e-c5ad-45b9-be23-71a2811317dd"
            }
          ]
        },
        {
          "id": "b2de2f14-ccfa-4875-9ff9-1e74795cd075",
          "name": "listIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPolicies?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad514f9a-f0a4-45cb-85c6-05d09f7685aa"
            }
          ]
        },
        {
          "id": "f83392c0-6339-4ee8-843c-e0aa8f0b4abf",
          "name": "putIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutIdentityPolicy?Identity=Identity&Policy=Policy&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or updates a sending authorization policy for the specified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e85a9d8b-b41f-4aed-8c9c-f93018f1e57f"
            }
          ]
        },
        {
          "id": "9d415ecf-7ca3-4827-852e-17e2393a3bde",
          "name": "setIdentityDkimEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityDkimEnabled?DkimEnabled=DkimEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables Easy DKIM signing of email sent from an identity:If Easy DKIM\n            signing is enabled for a domain name identity (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d8b4862-2cc7-4115-b81b-0a3d7cb84216"
            }
          ]
        },
        {
          "id": "f24ac4a9-0d27-4b2b-adf2-99d03c592206",
          "name": "setIdentityFeedbackForwardingEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityFeedbackForwardingEnabled?ForwardingEnabled=ForwardingEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), enables or disables whether Amazon SES forwards bounce and complaint notifications as email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baf3c54b-07a2-4fef-a350-94d6298cd7bb"
            }
          ]
        },
        {
          "id": "dcb62481-0317-47ab-90f3-e8ea97cf588d",
          "name": "setIdentityHeadersInNotificationsEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityHeadersInNotificationsEnabled?Enabled=Enabled&Identity=Identity&NotificationType=NotificationType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), sets whether Amazon SES includes \n            the original email headers in the Amazon Simple Notification Service (Amazon SNS) notifications \n            of a specified type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dadde6d-d2f5-4ef3-98cf-1cd54ea9f615"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "c6a57073-9f82-4385-9cfb-9bbacfa18687",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52ec0176-038c-47a0-86cb-2b6bfb854665"
            }
          ]
        },
        {
          "id": "eab48cb0-e591-4a59-9184-beef50ea542a",
          "name": "listVerifiedEmailAddresses",
          "request": {
            "url": "http://example.com/api/?Action=ListVerifiedEmailAddresses?VerifiedEmailAddresses.member.N=VerifiedEmailAddresses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the email addresses that have been verified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f58668c9-d4bb-438c-9aa2-4986e38211c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "fd6b46e4-b000-4fbb-a280-166c2d554924",
          "name": "getSendQuota",
          "request": {
            "url": "http://example.com/api/?Action=GetSendQuota?Max24HourSend=Max24HourSend&MaxSendRate=MaxSendRate&SentLast24Hours=SentLast24Hours",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's current sending limits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06ed5870-9228-40c1-a41d-a1192f9a4414"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "54ce776c-54c7-4ff0-8629-354025955e72",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab66fb23-46d5-436b-bba3-597ab97c46f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "74aa8114-6381-45f2-862c-1f1047f705ee",
          "name": "sendBounce",
          "request": {
            "url": "http://example.com/api/?Action=SendBounce?BouncedRecipientInfoList.member.N=BouncedRecipientInfoList.member.N&BounceSender=BounceSender&BounceSenderArn=BounceSenderArn&Explanation=Explanation&MessageDsn=MessageDsn&OriginalMessageId=OriginalMessageId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates and sends a bounce message to the sender of an email you received through Amazon SES."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "081a47d1-14ae-4547-915f-a156fd6a90d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Email",
      "item": [
        {
          "id": "0cb87a16-9666-4222-be35-438cda020842",
          "name": "sendEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendEmail?ConfigurationSetName=ConfigurationSetName&Destination=Destination&Message=Message&ReplyToAddresses.member.N=ReplyToAddresses.member.N&ReturnPath=ReturnPath&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Composes an email message based on input data, and then immediately queues the message for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0b9e5b5-851a-4329-8898-c45e7bbce98f"
            }
          ]
        },
        {
          "id": "5f1883be-8de9-41cc-abd5-dcb4936657b4",
          "name": "sendRawEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendRawEmail?ConfigurationSetName=ConfigurationSetName&Destinations.member.N=Destinations.member.N&FromArn=FromArn&RawMessage=RawMessage&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends an email message, with header and content specified by the client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b37fb144-c6fc-4abd-81de-a4339ffa05d9"
            }
          ]
        }
      ]
    }
  ]
}