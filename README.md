# PGTTool
PGameTrackerTool is a set of tools and api for games

## HOW IT WORKS
For now it works only with Minecraft status

```
<script src="https://cdn.jsdelivr.net/gh/kratess/PGTTool_api/PGTTool_api.js" charset="utf-8"></script>
<script type="text/javascript">
  PGTTool_api.getStatusMC("mc.hypixel.net",
  function(status, err) {
    if (status !== null) {
      document.getElementById("element").innerHTML = "TEST Minecraft - HYPIXEL online: " + status.online + " - optional - " + err;
    } else {
      //error
      document.getElementById("element").innerHTML = "NOT WORK - optional - " + err;
    }
  });
</script>
```

## API (Minecraft)

Status

```
status.online
status.min
status.max
status.last_update
```
