# game-dev-m2

# arrays random items
![2025-11-27-12-23-07](https://github.com/user-attachments/assets/e839136f-2c64-4f08-ae09-7a8c6de1a546)

[Uploading randomitem.cs…]()


    using UnityEngine;

     public class randomitem : MonoBehaviour
     {
 
    [SerializeField] string[] Items = new string[10]; 
 
          void Start()
           {
        Items[0] ="apple";
        Items[1] ="pear";
        Items[2] ="pineapple";
        Items[3] ="piza";
        Items[4] ="pommegranade";
        Items[5] ="cucumber";
        Items[6] ="mango";
        Items[7] ="bannana";
        Items[8] ="sugarapple";
              Items[9] ="orange";
        
     }        
    

    
    void Update()
    {

    
        if (Input.GetKeyDown(KeyCode.Return)) PrintRandomItem();
        if (Input.GetKeyDown(KeyCode.Escape)) PrintAllItems();
    }
    private void PrintRandomItem()
    {
        Debug.Log(Items[Random.Range(0, 9)]);
    }
    private void PrintAllItems()
    {
        foreach (var it in Items)
        {
            Debug.Log(it);
        }
    }
      }








#
