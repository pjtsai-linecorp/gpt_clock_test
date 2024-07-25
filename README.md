1. 幫我用html畫出一個時鐘的錶面，要有數字、時針和分針
<img width="466" alt="Screenshot 2024-07-25 at 6 19 08 PM" src="https://github.com/user-attachments/assets/0f27e47a-88a6-45ed-8f1f-a1b18fc8a300">

2. 時針和分針的原點不在圓心，另外，把1-12所有的數字都畫上去
<img width="387" alt="Screenshot 2024-07-25 at 6 22 33 PM" src="https://github.com/user-attachments/assets/c4a56edf-0447-4ec8-acd4-4fe89e534ce2">

3. 時針和分針的原點還是不對
<img width="377" alt="Screenshot 2024-07-25 at 6 23 26 PM" src="https://github.com/user-attachments/assets/69e4389f-b70a-421b-b839-c519b5db4bcd">

4. 時針和分針的位置對了，但我總覺得除了3, 6, 9, 12以外的數字位置怪怪的
<img width="407" alt="Screenshot 2024-07-25 at 6 23 57 PM" src="https://github.com/user-attachments/assets/c3879ec8-df02-45a6-9852-ae7c41b42b41">

5. 1和2沒有均勻分布在12和3之間，其他如4,5、7,8、10,11也是一樣
<img width="368" alt="Screenshot 2024-07-25 at 6 26 08 PM" src="https://github.com/user-attachments/assets/123694f6-198a-406b-b61a-79d5c86d1ea1">

6. 不錯，不過你可以讓數字再更靠近邊緣一點嗎
<img width="377" alt="Screenshot 2024-07-25 at 6 26 37 PM" src="https://github.com/user-attachments/assets/a78373ef-fdf7-4322-a649-f5cc45f1a3db">

7. 好，那麼我現在希望隨機生成一個時間，並顯示在時鐘上。另外給我一個輸入匡，和一個按鈕。當我按下按鈕的時候，檢查輸入匡裡輸入的時間跟時鐘上顯示的時間是不是一樣。
<img width="390" alt="Screenshot 2024-07-25 at 6 27 10 PM" src="https://github.com/user-attachments/assets/5f27cebd-2382-43a1-b009-2db1fa7b6f36">

8. (因為怎麼回答都錯，所以開始debug)我們先回到上一步，你隨機產生一個時間，顯示在時鐘上，另外找的地方印出這個時間來
<img width="370" alt="Screenshot 2024-07-25 at 6 27 46 PM" src="https://github.com/user-attachments/assets/14872683-69dc-4ec2-909d-b66e20ce1915">

9. 你的時鐘畫錯了吧，跟時間不一樣啊
<img width="406" alt="Screenshot 2024-07-25 at 6 28 26 PM" src="https://github.com/user-attachments/assets/cf274d6a-f235-4971-aa06-6545b48d50ec">

10. updateClock畫出來的時鐘時間和displayTime不一樣(updateClock和displayTime都是html裡的js function)
<img width="399" alt="Screenshot 2024-07-25 at 6 28 59 PM" src="https://github.com/user-attachments/assets/a706b38e-16e9-4db7-9a8b-64014ff94b21">

11. 來，我們先從分針開始，亂數時間是幾分時鐘上就把分針指到對應的地方
<img width="366" alt="Screenshot 2024-07-25 at 6 29 31 PM" src="https://github.com/user-attachments/assets/667b89a7-b49f-4dfb-943d-c53eddd4e1ce">

12. 你給的程式碼，當時間為0分的時候，分針是指在哪個數字
<img width="362" alt="Screenshot 2024-07-25 at 6 30 14 PM" src="https://github.com/user-attachments/assets/cf6db583-9f4d-4a30-8c9d-f696b33f3332">

13. 但是我試了一下，當minutes為0的時候，指針是指在3
<img width="376" alt="Screenshot 2024-07-25 at 6 31 15 PM" src="https://github.com/user-attachments/assets/30c21e10-a6d5-4890-bf07-a28e949a1f69">

14. (這一步我真的開code看，也是唯一碰code的一步）還是不對，你要不要試試看把分針的rotation減少90度？
<img width="374" alt="Screenshot 2024-07-25 at 6 31 48 PM" src="https://github.com/user-attachments/assets/320c4aa1-d44e-4e3d-b20d-1ac23af460b7">

15. 看起來ok，現在把時針加上去。注意不要犯了跟畫分針時一樣的錯誤了
<img width="347" alt="Screenshot 2024-07-25 at 6 32 22 PM" src="https://github.com/user-attachments/assets/a30d2d9b-ef70-44a0-b064-97d2c57ff017">

16. 好，那現在幫我放上輸入匡和檢查鈕
<img width="382" alt="Screenshot 2024-07-25 at 6 32 52 PM" src="https://github.com/user-attachments/assets/c0b70021-f591-466f-8934-c520256f04f2">

17. 拿掉顯示的答案，把訊息都改成繁體中文和台灣用語。如果答錯的話，顯示正確答案。
<img width="371" alt="Screenshot 2024-07-25 at 6 33 23 PM" src="https://github.com/user-attachments/assets/e2434a23-7540-4268-84bc-21758c006c34">

18. 再幫我加個按鈕，按下去是出題
<img width="385" alt="Screenshot 2024-07-25 at 6 34 32 PM" src="https://github.com/user-attachments/assets/48c57b03-9934-45dc-a8c5-5f1bae04ff24">
