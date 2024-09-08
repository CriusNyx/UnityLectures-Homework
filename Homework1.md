# Question 1

1. Create a component called Health.

```c#
using UnityEngine

public class Health: MonoBehaviour{

}
```

2. Create a public float called currentHealth and maxHealth.

3. On Start set current health to max health

4. Create an enum called HealthType

```c#
public enum HealthType{

}
```

5. Create two possible values for HealthType

- playerHealth
- enemyHealth

6. Add the following method to Health

```c#
void OnTriggerEnter2D(Collider2D collider){

}
```

7. Make it so that anytime the health component collides with the bullet the following happens.

- The health checks to see if the thing that hit is has a Hitbox
- The health checks to see if that Hitbox is able to damage this health
- If the Hitbox is able to damage it the health gets decreased by 1.
- If the health is 0 or less it Destroys the gameObject.

8. Attach the health component to Player and to Enemy.

9. Remove the existing code from Player and Enemy to manage health. Let the Health component do all the work.
