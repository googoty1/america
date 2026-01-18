# america
using UnityEngine;

public class freecam : MonoBehaviour
{
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        float DT = Time.deltaTime;
        float speed = 20f;

        if (Input.GetKeyDown(KeyCode.W) = true)
        {
            transform.Translate(Vector3.forward * speed * DT);
        }

        else if (Input.GetKeyDown(KeyCode.S))
        {
            transform.Translate(Vector3.back * speed * DT);
        }

        else if (Input.GetKeyDown(KeyCode.A))
        {
            transform.Translate(Vector3.left * speed * DT);
        }

        else if (Input.GetKeyDown(KeyCode.D))
        {
            transform.Translate(Vector3.right * speed * DT);
        }
    }
}
