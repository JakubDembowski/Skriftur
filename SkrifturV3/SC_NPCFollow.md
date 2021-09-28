```c#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class SC_NPCFollow : MonoBehaviour
{
    //Transform lætur NPC að elta
    public Transform transformToFollow;
    //NavMesh Agent
    UnityEngine.AI.NavMeshAgent agent;

    // Start is called before the first frame update
    void Start()
    {
        agent = GetComponent<UnityEngine.AI.NavMeshAgent>();
    }

    // Update is called once per frame
    void Update()
    {
        //Elta Player
        agent.destination = transformToFollow.position;
    }
}

// Script eftir Jakub K. Dembowski
```
