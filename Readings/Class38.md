## Intent Filters

- Three criteria an activity's intent filter must fulfill:

1. Action: It should specify the action to perform, like ACTION_SEND or ACTION_VIEW.
2. Data: It should describe the type of data associated with the intent, such as a MIME type or URI scheme.
3. Category: It provides additional characteristics of the activity, usually set to CATEGORY_DEFAULT.

- How an activity retrieves the Intent it was started by:

Call getIntent() within the activity's code, typically during early lifecycle callbacks like onCreate() or onStart().
This method returns the Intent that started the activity.
You can then examine the intent to determine the action, data, and other details.

- Explaining intents to a non-technical friend:
Think of intents as messages between different parts of a smartphone.
An intent is like an envelope containing instructions (action) and information (data).
Apps can send and receive these envelopes, allowing them to work together.
For example, if you want to share a picture from your gallery, the gallery app sends an intent to the messaging app saying, "I have a picture to share." The messaging app then opens, ready to receive and send that picture.


- Compare and contrast implicit and explicit intents:

- Explicit Intents:

Specify the target app's package name or a fully-qualified component class name.
Used for starting a specific component within your own app.
Directly invokes a known component (activity, service, etc.) in your app.
Generally used when you have a clear idea of the component you want to start.

- Implicit Intents:

Do not specify a specific component but declare a general action to perform.
Allow components from other apps to handle the intent.
Useful when the target app is not known, and you want other apps to respond based on the declared action.
The system determines the appropriate component based on the intent's action, data, and other properties.

- Primary information contained within an Intent:

1. Component Name: The name of the component to start (optional for implicit intents, critical for explicit intents).
2. Action: A string specifying the generic action to perform (e.g., ACTION_VIEW or ACTION_SEND).
3. Data: The URI (a Uri object) referencing the data to be acted upon and/or the MIME type of that data.
4. Category: Additional information about the kind of component that should handle the intent (e.g., CATEGORY_LAUNCHER).
5. Extras: Key-value pairs carrying additional information required to accomplish the requested action.
6. Flags: Metadata for the intent, instructing the system on how to launch and treat the activity.