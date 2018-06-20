{
  "info": {
    "name": "Foursquare Post Updates Marknotificationsread",
    "_postman_id": "5e6d9375-3785-4dc3-99eb-1771e03247d5",
    "description": "/updates/notifications",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "14b5fa78-51c2-47e0-8d62-b6125e408188",
          "name": "campaignscampaign-id",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/add?campaignId=%7B%7D&endAt=%7B%7D&groupId=%7B%7D&specialId=%7B%7D&startAt=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e805d39a-5028-421c-84d7-9c42a826b7bc"
            }
          ]
        },
        {
          "id": "3d74eec6-12c9-43df-a4db-d9cfe8716c98",
          "name": "campaignsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/list?groupId=%7B%7D&specialId=%7B%7D&status=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c2d8ffc-a28e-4531-9725-8f772f99bdff"
            }
          ]
        },
        {
          "id": "04fede90-2393-4db8-876f-f90ca2cd2b1d",
          "name": "specialsspecial-idretire",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/retire"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13272d9d-6a34-4d20-9693-c954393284b1"
            }
          ]
        },
        {
          "id": "f7d8b481-b2db-4277-95ca-37d695599a00",
          "name": "campaignscampaign-idtimeseries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/delete"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/timeseries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee9b5f38-6eae-48d6-9f17-b46533fcda1a"
            }
          ]
        },
        {
          "id": "167d96a9-1906-49de-a3d1-0973b6b6a363",
          "name": "campaignscampaign-iddelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/end"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/delete"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2fda8ef-caac-4d45-bae3-2cf9365f130d"
            }
          ]
        },
        {
          "id": "59ec179b-4dd6-4f1c-a745-0345dc64b558",
          "name": "campaignscampaign-idend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/start"
              ],
              "query": [
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/end"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54e3bb1d-8a91-450c-9ce6-f42c1e484f2a"
            }
          ]
        },
        {
          "id": "e94780d0-4913-40a0-836a-7eb0e8a9e486",
          "name": "campaignslist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/timeseries"
              ],
              "query": [
                {
                  "key": "endAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ea5e1c7-aa57-4d4c-be94-e33009198c06"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkins",
      "item": [
        {
          "id": "984eec9a-e9d7-4a78-96c1-b876abe00110",
          "name": "checkinscheckin-id",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&eventId=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&shout=%7B%7D&v=%7B%7D&venue=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc653c10-b963-49e3-b495-a871d2f1db7c"
            }
          ]
        },
        {
          "id": "c71f8ad0-6f7e-4393-b451-b9f3269f34da",
          "name": "checkinsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/recent?afterTimestamp=%7B%7D&limit=%7B%7D&ll=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "052bb526-1172-4d66-bb0d-fe2ae8d84d50"
            }
          ]
        },
        {
          "id": "d0591857-6408-4cfb-9da0-b995c2db1481",
          "name": "venuegroupsgroup-idremovevenue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID"
              ],
              "query": [
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}/removevenue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "651e2f25-2701-48f5-b5be-920fb00cbd3e"
            }
          ]
        },
        {
          "id": "ec3997f8-ca20-4176-9703-5f566141e30e",
          "name": "checkinsrecent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/addcomment"
              ],
              "query": [
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/recent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "736573bd-3247-4975-b743-279b6afe6fad"
            }
          ]
        },
        {
          "id": "8e6705d9-2171-4a69-9373-ed39e09758ab",
          "name": "checkinscheckin-idaddcomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/deletecomment"
              ],
              "query": [
                {
                  "key": "commentId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/addcomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1474650-c345-47fa-ba5f-e7bc6216d73f"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "e9f4c5ba-7236-405a-85c9-3eed0cc96897",
          "name": "eventsevent-id",
          "request": {
            "url": "http://api.foursquare.com/v2/events/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/{EVENT_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf514b65-a170-4bc8-8f24-5e89cea35ca8"
            }
          ]
        },
        {
          "id": "1782a9c6-c79b-495d-bd46-3e0158d83e4b",
          "name": "eventscategories",
          "request": {
            "url": "http://api.foursquare.com/v2/events/search?domain=%7B%7D&eventId=%7B%7D&participantId=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eae316f7-5452-4703-a2ef-7f29d2c000cb"
            }
          ]
        },
        {
          "id": "f3d17b04-08c1-4f4b-9a5c-cb82683edbe7",
          "name": "campaignscampaign-idstart",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "events/:EVENT_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "EVENT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/start"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "475d0182-8be7-4e06-ae07-afb1863d8b80"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "3b6d7261-c8af-4060-ae1d-4d84ad6a8d10",
          "name": "listslist-id",
          "request": {
            "url": "http://api.foursquare.com/v2/lists/add?collaborative=%7B%7D&description=%7B%7D&name=%7B%7D&photoId=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "864773e3-b877-488c-9d2f-90910e61490b"
            }
          ]
        },
        {
          "id": "c15b1754-d9f1-4a13-a1df-a1958d442f15",
          "name": "tipstip-idunmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/unmark"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6a2563c-8755-49cb-bb6c-feeb8545582d"
            }
          ]
        },
        {
          "id": "de1fec4b-b14b-4594-93c4-923835ab4c8c",
          "name": "listslist-idsuggestvenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/additem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "listId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestvenues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cb699b5-7025-46c5-bbd1-2cd71600eabf"
            }
          ]
        },
        {
          "id": "6d04dcd3-6a5b-4961-b3de-dd99b57a3181",
          "name": "listslist-idadditem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/deleteitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/additem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6c67dd4-d92e-4232-86e4-a282c2f3ff1f"
            }
          ]
        },
        {
          "id": "8eae066f-053a-4368-b27d-9f12a789d6ae",
          "name": "listslist-iddeleteitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/follow"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/deleteitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9e46ecb-2879-4984-9593-17657cd54e7a"
            }
          ]
        },
        {
          "id": "06367143-021d-4304-b4ea-40b7958ebe89",
          "name": "listsadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/followers"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "317192d8-6176-465d-bffa-9ac20a8ffd66"
            }
          ]
        },
        {
          "id": "25c91ba0-f469-4d39-9fdc-bdcc0265403a",
          "name": "listslist-idfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/moveitem"
              ],
              "query": [
                {
                  "key": "afterId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "beforeId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/follow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1187569d-f019-4c91-8f77-8e8fe581249a"
            }
          ]
        },
        {
          "id": "a8dfded3-b043-419c-9246-bc339ef6cb60",
          "name": "listslist-idmoveitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/share"
              ],
              "query": [
                {
                  "key": "broadcast",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/moveitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f89ab835-6ccd-4047-83e8-fa547d5ffc4a"
            }
          ]
        },
        {
          "id": "89345d21-02b5-45b0-9854-63f22ff21c8d",
          "name": "listslist-idfollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestphoto"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/followers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b100036-8472-4b24-96bc-93a16f32d0a4"
            }
          ]
        },
        {
          "id": "33ac9cf9-98ef-465e-9abe-a749ba121ca1",
          "name": "listslist-idsuggestphoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggesttip"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestphoto"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c26ac904-2b85-4c6a-8e8e-cb832b6c16f7"
            }
          ]
        },
        {
          "id": "8df0501d-2ee4-470d-91b1-ed8e974062d9",
          "name": "listslist-idsuggesttip",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestvenues"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggesttip"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d8fd623-16ee-49e8-904f-0ca5aa74f4fc"
            }
          ]
        },
        {
          "id": "39413c94-433a-4bd1-b819-32904e324719",
          "name": "listslist-idshare",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/unfollow"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/share"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ab3f627-bdfe-4e25-a820-e4a84a374e86"
            }
          ]
        },
        {
          "id": "f030dfe6-4854-4353-9fbe-8296382a6145",
          "name": "listslist-idunfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/update"
              ],
              "query": [
                {
                  "key": "collaborative",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/unfollow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d52c7b60-1325-4a9c-a837-5f81613f12d4"
            }
          ]
        },
        {
          "id": "23780342-69f3-41f5-b791-c7be8ed0d973",
          "name": "listslist-idupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/updateitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e88ab21-4aac-40c7-aa1e-b8d95d5b6d41"
            }
          ]
        }
      ]
    },
    {
      "name": "Multi",
      "item": [
        {
          "id": "1b4beac0-a841-473b-b0b7-de8868af18c8",
          "name": "pagespage-idvenues",
          "request": {
            "url": "http://api.foursquare.com/v2/multi?requests=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}/venues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "058cb210-ad78-4fc2-b396-fd3689d98b30"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "4ff22486-aca7-49c7-a35b-fa955f94f9bf",
          "name": "pagespage-id",
          "request": {
            "url": "http://api.foursquare.com/v2/pages/search?fbid=%7B%7D&name=%7B%7D&twitter=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b29913c4-5f37-4577-9c9a-87ddec6f28e4"
            }
          ]
        },
        {
          "id": "7ba5c779-5d1b-4d83-9d91-7af6a6086752",
          "name": "eventssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62fdb1fa-411e-42ed-9007-be8c279f5c16"
            }
          ]
        },
        {
          "id": "e33a6b80-777d-464f-a861-9d41d6c7c45c",
          "name": "pagessearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID/venues"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ne",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "radius",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sw",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9636dc33-00ab-4328-9d3a-0d30190779eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "e4357e20-9f43-4a2b-8384-7caf0d6e4edc",
          "name": "photosphoto-id",
          "request": {
            "url": "http://api.foursquare.com/v2/photos/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&checkinId=%7B%7D&Content-Type=%7B%7D&image=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&public=%7B%7D&tipId=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/{PHOTO_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bb11b3a-66d3-4cc7-92c4-1ee8909d3a28"
            }
          ]
        },
        {
          "id": "51ba0027-693b-4ac5-a677-f0a414c37cf8",
          "name": "updatesmarknotificationsread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "photos/:PHOTO_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PHOTO_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/marknotificationsread"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07f0f4ab-4c3e-43f5-8bc6-11afda620da4"
            }
          ]
        }
      ]
    },
    {
      "name": "Settings",
      "item": [
        {
          "id": "24224cc2-a3a7-4364-8e90-46f7cd09362d",
          "name": "settingssetting-id",
          "request": {
            "url": "http://api.foursquare.com/v2/settings/all?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a51aca3-947a-43f1-9114-8e38e357e418"
            }
          ]
        },
        {
          "id": "c977a643-4d2e-4053-8d52-8c02b9a1f1f8",
          "name": "photosadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "948b6eb6-563e-4ebc-9673-52d163f6f53d"
            }
          ]
        },
        {
          "id": "e3a602da-372c-45f3-9f27-fe862e0f7ecf",
          "name": "settingsall",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID/set"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a2d3694-e3cc-4315-9d7c-9d504fe478bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Specials",
      "item": [
        {
          "id": "1c37c6ee-a877-4146-af55-05c2a3e342b2",
          "name": "specialsspecial-id",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/add?cost=%7B%7D&count1=%7B%7D&count2=%7B%7D&count3=%7B%7D&finePrint=%7B%7D&name=%7B%7D&offerId=%7B%7D&text=%7B%7D&type=%7B%7D&unlockedText=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77bc4439-d2ff-4d24-8630-ec28aeb26ea4"
            }
          ]
        },
        {
          "id": "d22dfec9-e153-4a91-afaa-0388ddb9581c",
          "name": "specialsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/list?status=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7267204-d39a-42cb-949e-39fcfca249c3"
            }
          ]
        },
        {
          "id": "49583cdd-7d62-4e80-92b6-f2526943c07b",
          "name": "specialslist",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/search?alt=%7B%7D&altAcc=%7B%7D&limit=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&radius=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "425106d7-1187-427a-8a2a-4f1f3ffd33af"
            }
          ]
        },
        {
          "id": "9115d0e6-6cef-4a77-9a53-0f14b90a649e",
          "name": "specialsspecial-idconfiguration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:ID/flag"
              ],
              "query": [
                {
                  "key": "problem",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64866419-3b89-4e74-bb1c-4c2fcbd782ff"
            }
          ]
        },
        {
          "id": "59446e27-c0a5-4465-a8c0-243295d93034",
          "name": "settingssetting-idset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}/set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "174471fb-29fb-4bbb-93ad-709eee69d712"
            }
          ]
        },
        {
          "id": "710e16c3-dd87-42c4-b024-bcbf3ad6cfdb",
          "name": "specialssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/configuration"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f7ef3ba-aee9-4751-980a-b7837533b0ca"
            }
          ]
        },
        {
          "id": "ccf9dfe6-18f5-482c-bbd9-092e9c964f6d",
          "name": "specialsidflag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/retire"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{ID}/flag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3553d4b-6705-4d93-accc-55606bbac3c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Tips",
      "item": [
        {
          "id": "82732493-172a-48c2-8450-e758c2ffcfbb",
          "name": "tipstip-id",
          "request": {
            "url": "http://api.foursquare.com/v2/tips/add?broadcast=%7B%7D&text=%7B%7D&url=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28984449-2ed2-4790-bb3d-15bdb680be7c"
            }
          ]
        },
        {
          "id": "d46b5bca-7256-4bbc-9248-e26193359e62",
          "name": "tipsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/tips/search?filter=%7B%7D&limit=%7B%7D&ll=%7B%7D&offset=%7B%7D&query=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bde8b627-926a-4806-8695-f46b135edaa5"
            }
          ]
        },
        {
          "id": "27a4b318-5b02-43e0-b5f9-f5f4b0f2c654",
          "name": "checkinscheckin-iddeletecomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/deletecomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6fa754e-490b-4260-a4fe-591366e06538"
            }
          ]
        },
        {
          "id": "c4d8b101-058c-493e-b424-9df41a763a86",
          "name": "tipssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/done"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a34c7a84-eb10-4ccb-84d1-5b81536f56bf"
            }
          ]
        },
        {
          "id": "8311acb1-8fed-4fbc-b095-d8ade4206397",
          "name": "tipstip-iddone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/listed"
              ],
              "query": [
                {
                  "key": "group",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/done"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69bf6b07-ddba-446b-8d3c-ec37608c44f1"
            }
          ]
        },
        {
          "id": "1dec7530-1af6-4af3-b6d3-f4aba5924cd2",
          "name": "tipstip-idlisted",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/markdone"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/listed"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df170de5-612f-44b6-b06b-2a7c821dc272"
            }
          ]
        },
        {
          "id": "60dca5b5-a688-413f-96a4-9273fed14c12",
          "name": "tipstip-idmarkdone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/marktodo"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/markdone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a64b18d-6e45-44f0-a6ee-d58b1c934dad"
            }
          ]
        },
        {
          "id": "380ac84c-da98-4eb2-893e-1d3f8e4c370d",
          "name": "tipstip-idmarktodo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "tips/:TIP_ID/unmark"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TIP_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/marktodo"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42933346-24e9-49f1-bd31-4b4014cc96cf"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "ae5f8fc9-6411-4bc2-8bf8-4fbabb16c2ed",
          "name": "updatesnotifications",
          "request": {
            "url": "http://api.foursquare.com/v2/updates/marknotificationsread?highWatermark=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/notifications"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f5e984f-b233-4f61-8173-2b55b91c4a75"
            }
          ]
        }
      ]
    }
  ]
}