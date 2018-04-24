
Here you can read about my current problem with the maxcube in HA:

https://community.home-assistant.io/t/maxcube-loosing-configuration/46663)

The maxcube-py file is a copy of the maxcube component in home-assistant.
I have added the option to configure the update interval.

To use it place it in a custom_components folder in your HA configuration folder - this will override the build-in maxcube component.

You can add an "update_interval" to the configuration like this:

```yaml
maxcube:
  host: 192.168.1.4
  update_interval: 300
```

The update_interval is in seconds - so 300 is 5 minutes.

This is a temporary solution to test if it will actually fix the issue in HA.
It can take several week for the reset to happen, so I want to make sure before I make a more permanent solution.
