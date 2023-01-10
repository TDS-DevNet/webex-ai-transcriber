# Webex Meeting API
https://developer.webex.com/docs/api/v1/meeting-transcripts

Test Meeting API here
https://developer.webex.com/docs/api/v1/meeting-transcripts/download-a-meeting-transcript

## How to integrate with Webex
https://developer.webex.com/docs/integrations

## Webex meeting transcripts - setup and manually download
Transcripts: To create a transcript, you must turn on Webex Assistant. This cannot be done programmatically and must be turned on by the meeting host/participant or set as default behavior in the control hub. NOTE: Webex Assistant requires a license.

https://help.webex.com/en-us/article/r0jptm/Review-and-manage-meeting-transcripts-created-by-Webex-Assistant-for-Meetings
https://help.webex.com/en-us/article/npoakae/Download-a-recording-transcript-for-Webex-meetings,-webinars,-and-events
https://developer.webex.com/blog/accessing-meeting-resources-from-webex

## Access Meeting Resources Guide

Get the Transcripts – VTT and TXT format

You can now query for the transcripts using endpoint:- `/v1/meetingTranscripts/`

A query might look like: `https://webexapis.com/v1/meetingTranscripts?meetingId=501e995485e2460bb129410116757b13_I_194316955237236650`

This will return to something like this:

```
{
    "items": [
        {
            "id": "a5038f0b-320a-456f-a51f-7541eeb0eae5_M_501e995485e2460bb129410116757b13",
            "meetingId": "501e995485e2460bb129410116757b13_I_194316955237236650",
            "startTime": "2021-05-14T20:25:22Z",
            "vttDownloadLink": "https://webexapis.com/v1/meetingTranscripts/a5038f0b-320a-456f-a51f-7541eeb0eae5_M_501e995485e2460bb129410116757b13/download?meetingId=501e995485e2460bb129410116757b13_I_194316955237236650&format=vtt",
            "txtDownloadLink": "https://webexapis.com/v1/meetingTranscripts/a5038f0b-320a-456f-a51f-7541eeb0eae5_M_501e995485e2460bb129410116757b13/download?meetingId=501e995485e2460bb129410116757b13_I_194316955237236650&format=txt"
        }
    ]
}
```

>Resource: https://developer.webex.com/docs/api/guides/access-meeting-resources-guide

