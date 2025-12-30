Displays a formatted summary of all "automation override" switches when they are active ("ON").  We have Global, Area, Device, and Special (assigned to my wife) override helpers. When having a party, everything is overridden (door lock, lighting, motion, etc.).  When one of you wants to sleep in the other can override just the bedroom motion sensor for you.
**Main Card:** custom:auto-entities
**Embedded Cards:** custom:mushroom-template-card
**Modifiers:** card-mod
**Extra Steps:** Requires the addition of attributes to the input_boolean helpers via config. Then the entities can be filtered by the auto-entities card.  The method is used again in an Area Card Plus card (posted separately.   (Will post thanks and attributions in a bit - new to github.)

**Examples:**
homeassistant:
  customize:
    input_boolean.all_automation_off:
      monitored_override: true
      override_category: "Global"
    input_boolean.lr_motion_off:
      monitored_override: true
      override_category: "Area"
    input_boolean.garage_door_automation_off:
      monitored_override: true
      override_category: "Device"
      
