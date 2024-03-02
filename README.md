# Tutos-clouformation-Pipeline
Plusieurs questions sont posées de savoir comment faire du pipeline avec cloudformation, si vous vous posez la même question alors ce tuto est fait pour vous ! Dans ce tutos nous allons apprendre comment deployer notre infrastructure ec2 avec pipeline . nous allons utilisé le même code pour cet exercice . let's go! 
Pour ce faire il faut créer un rôle pour cloud formation en ajoutant l'accès à AmazonEC2FullAcess . pour créer le rôle il faut utilisé le service IAM pour ça;

![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/895cf57d-d14f-4c0a-be16-1eab42f4041d)




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/b9f3bef7-7f85-4fa8-a39a-b2a6b7827787)





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/82c9aaa3-48f2-4a9c-9081-3bfe09275f2a)



Choisissez Cloud formation comme option;
Ensuite cliquez sur suivant;



![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/fbc7533c-e89d-43f5-87b3-3bcc11f000bd)





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7a806e7f-15ec-4fe5-9802-60ce8a280df8)




Cliquez sur suivant;
Ensuite nomez votre rôle;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/c1bd9772-2522-4a8f-ad56-a9ff4d1175c3)





Cliquez sur créer un rôle;
Ensuite allez dans code commit, code commit nous permettra d'éxecuter notre code à partir du pipeline . Nos text se feront dans code commit;





![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/7a0db6a8-f797-49bd-8222-21dce608446c)






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/3849de3a-66d7-4958-907f-5b2133f3658a)




Il faut créer un référentiel;




![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/2d3b9522-3cbb-42c1-9dbd-b478c508de3c)






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/6cd810ae-4a8a-4e61-be2b-3569901a4333)





Dans l'option ajouter un fichier vous allez cliquer charger un fichier . comme je le dis au départ nous allons utilisé le même fichier(instance.yml);






![image](https://github.com/AWS-Re-Start-RDC-KINSHASA-1/Tutos-clouformation-Pipeline/assets/114914329/bdee6537-c747-4e2e-bca9-75b3f4e97a5b)










