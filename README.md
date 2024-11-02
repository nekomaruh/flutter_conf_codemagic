# Flutter Conf LATAM - Codemagic CI/CD Workshop

The base project was presented by Ignacio Lauret, who explained a way to implement CI/CD with CodeMagic in Flutter. In the source you can get more information on how to implement new configurations.

Source: https://github.com/ignalauret/codemagic_flutter_conf


# 1. Create File

This project exposes a way to create continuous integration with codemagic, it is very simple, you just have to configure a file named codemagic.yaml, which will contain the configuration that must be linked in codemagic.

<img width="486" alt="Captura de pantalla 2024-11-02 a la(s) 10 06 21" src="https://github.com/user-attachments/assets/a0c46f91-dc5b-41c7-a67b-7dbf4526e8df">

# 2. Link source code

In this case we use GitHub as the code source, this is also where we add the configuration from our repository to CodeMagic and we just have to copy and paste the link of the project (it should be public).

<img width="1725" alt="Captura de pantalla 2024-11-02 a la(s) 10 13 23" src="https://github.com/user-attachments/assets/8006675d-f0bd-4a85-8ae7-251d279e85d8">


# 3. Add webhook

To notify the application via email, we will need to create a webhook in the GitHub configuration, note that the yaml configured at the beginning must contain the email address to which the notification should be sent. There is also support for other platforms that can run webhooks, such as Slack.

<img width="1720" alt="Captura de pantalla 2024-11-02 a la(s) 10 18 05" src="https://github.com/user-attachments/assets/fbc18e26-8e99-4589-80ea-4fcca850568d">


# 4. Run pipeline

The pipeline reviews the application, checks with syntactical analysis if there are any errors, tests the functions, and as a result generates versions of applications for android (apk) and ios (ipa), which can be executed by experienced testers or QA's.
 
<img width="1310" alt="Captura de pantalla 2024-10-30 a la(s) 12 11 21" src="https://github.com/user-attachments/assets/b5172c86-885b-4aa9-b6be-11174dd38942">

# 5. Review App

It also includes an email alert every time a new version of the application is exported. Log notes can also be added if necessary if an error occurs in the process.

<img width="646" center="true" alt="Captura de pantalla 2024-10-30 a la(s) 12 12 06" src="https://github.com/user-attachments/assets/6f2be9c6-3dcc-4664-b4f6-a66c36737f5f">
