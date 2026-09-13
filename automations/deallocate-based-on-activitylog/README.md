# Deallocate VM based on Activity Log

A machine shut down from inside Windows or Linux is stopped, still allocated on a host, and
still billed for compute. This watches for exactly that event and deallocates the machine a few
minutes later. One alert rule, one Logic App, no schedule and no tags.

This is the template behind the **Deploy to Azure** button.

**The full documentation lives beside the Bicep template:**
[what it creates, how it decides, what the identity may do, and the runs that verified it](https://github.com/simon-vedder/bicep/tree/main/automations/deallocate-based-on-activitylog).

## Verified

12 September 2026, against a Standard_B1s Ubuntu VM shut down from inside the guest. All three
variants deallocate a guest shutdown and leave an `az vm stop` alone.

## Read on

- [The write-up](https://simonvedder.com/deallocate-vm-based-on-activity-log/), how it was built
- [The tool page](https://simonvedder.com/tools/deallocate-on-activity-log/)
