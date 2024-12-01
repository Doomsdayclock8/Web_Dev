Write ! And it pops up. Clicking it gives you boilerplate code
![[Pasted image 20241201200311.png]]
![[Pasted image 20241201200324.png]]

# Emmet not working in VS Code 

[#vscode](https://dev.to/t/vscode)[#emmet](https://dev.to/t/emmet)[#json](https://dev.to/t/json)[#howtofix](https://dev.to/t/howtofix)

Emmet is a powerful extension in Visual Studio Code. If you are developing a website or working with any language such as HTML, Emmet helps you to write your code fast and efficiently without making silly mistakes.

But sometimes, while updating VS Code, the VS Code loses the file associations or Emmet stops working for some reason. I encountered the similar problem after I updated my VS Code. I was not able to use Emmet and it seemed annoying to me because I didn’t want to write whole html starter templates while working on website development. So I started finding out the solution and figured out how to fix that.

Step 1: Start your VS Code. Click on the Settings or press **Ctrl+,** to open the VS Code Settings.

Step 2: Click on the Extensions tab on the left side of the settings. Click on HTML.

Step 3: Click on the **_“Edit in settings:json”_** hyperlink to edit the settings in JSON format.

[![vscode_emmet.png](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fviby7si4nyryw1vg6yep.png)](https://media2.dev.to/dynamic/image/width=800%2Cheight=%2Cfit=scale-down%2Cgravity=auto%2Cformat=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fviby7si4nyryw1vg6yep.png)

Step 4: Inside the curly braces, enter the following code under the already written JSON code:

```


“emmet.triggerExpansionOnTab”: true,
“files.associations”: {“*html”: “html”},
"emmet.useInlineCompletions": true


```

Step 5: Save the file. Now if you try to apply Emmet in your code, it will work smoothly!!

That’s how I fixed this Emmet not working problem which I encountered when I updated VS Code. I hope this solution may be helpful for you as well and serves the purpose.