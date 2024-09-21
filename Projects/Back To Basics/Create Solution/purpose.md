## Purpose of Solutions:

- Transport apps and components between organizations.
- Apply customizations to existing apps.


## Components of a Solution:

- Can include apps, site maps, entities, processes, web resources, option sets, etc.
- Components are organized hierarchically (e.g., entities contain forms, fields, relationships).


## Types of Solutions:

- **Managed Solutions:**
    - Can be uninstalled; all components are deleted.
    - Cannot be imported back into the original organization.

- **Unmanaged Solutions:**
    - Components added to the default solution; cannot be deleted by uninstalling.
    - Overwrites existing customizations.


## Solution Layering:

**System Solution:** Default components in every organization.
**Managed Solutions:** Modify system components; last installed solution wins in conflicts.
**Unmanaged Customizations:** User-created changes; can be customized unless managed properties restrict them.

- **_Application Behavior_** : Default solution plus any managed solutions plus any unmanaged customizations you have applied will be reflected on the application.


## Managed Properties:

- Metadata that limits customization of certain components.


## Solution Dependencies:

- Solutions can depend on components from other solutions.
- You must install base solutions before dependent solutions.
- Base solutions cannot be uninstalled while dependent solutions are installed.