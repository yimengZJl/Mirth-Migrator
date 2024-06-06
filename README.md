
<p align="center"><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/71503553-2554-4e7c-8ec1-6de1ec953973" width="200"></p>
A tool that automates the migration of <a href="https://www.nextgen.com/solutions/interoperability/mirth-integration-engine/mirth-connect-downloads" target="_blank">Mirth Enterprise Service Bus</a> channels and code templates from one instance to another.
<h2>Features</h2>
<ul>
  <li><b>Code Templates and Channel Migration</b><br/>Code templates, channels, and even entire Channel Groups or Code Template Libraries can be migrated between Mirth instances with a single click. Code templates of directly or indirectly referenced functions can be automatically migrated with the channels.<br/><br/>
If a component already exists at the destination instance, conflict handling will be activated. The component to be migrated will be compared with the corresponding component of the target system, and the user can choose to skip its migration or overwrite the one on the target side.</li>
  <li><b>Meta Data and Source Code Viewing</b><br/>When a component is selected, important metadata and the source code are displayed.</li>
  <li><b>Documentation</b><br/>Upon clicking on a component, the relevant documentation is displayed. In the case of functions, this may include their descriptions, parameter definitions, and expected return values. In the case of channels, this may include a description and a change history. Multiple functions in one code template will be displayed as separate items.</li>
  <li><b>Compare</b><br/>If a component selected at one instance already exists at the other instance, it will be highlighted, and a compare button will appear. The source code and metadata for components can be compared in two ways: side-by-side or inline.</li>
  <li><b>Function Dependency Checking</b><br/>For each function, it is indicated which other functions it uses, as well as the channels and/or functions through which it is used.</li>
  <li><b>Channel Dependency Checking</b><br/>For each channel, either directly or indirectly referenced functions are shown. It is further indicated which code template libraries it references and if these references are correct. Non-needed as well as missing library references are highlighted</li>
   <li><b>Web-Based Application</b><br/>Mirth Migrator is a fully web-based application provided via a Mirth channel. There is no need for a separate user management system as it utilises the user pool of the Mirth installation, which runs the channel.</li>
<h2>Screenshots</h2>
  <kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/01fb4697-c3b1-4927-83b5-3880f2cad292" width="160"></kbd>
  <kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/582d4991-04b5-4132-805d-48aee2267c80" width="160"></kbd>
  <kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/0858502d-2135-4674-bdac-e784ab8fc1af" width="160"></kbd>
  <kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/d6752f34-d959-46cf-bbc8-e744b9284a47" width="160"></kbd>
  <kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd>

<h2>Installation</h2>

<table>
  <tr><td><b>1.</b></td><td>Copy the <b>folder "web"</b> to your Mirth installation (to <b>"&lt;Your Install Path&gt;\Mirth Connect"</b>)</td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>2.</b></td><td>Open the <b>menu item "Settings"</b>, there the <b>tab "Resources"</b> and press <b>"Add Resources"</b></td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>3.</b></td><td>In the field <b>Directory</b> enter <b>"./web/MirthMigrator/jar"</b> and <b>name</b> the new Resource <b>"MirthMigrator"</b></td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>4.</b></td><td><b>Save</b> the change and <b>press "Reload Resource"</b>.<br/>
    Depending on your Mirth version it should now show something like "&lt;Your Installation Path&gt;/Mirth%20Connect/web/MirthMigrator/jar/MirthMigrator.jar" or just "MirthMigrator.jar" under "Loaded Libraries"</td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>5.</b></td><td>Now go to menu item "<b>Channels</b>" and press "<b>Import Channel</b>"</td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>6.</b></td><td>Import <b>MIRTH_MIGRATOR.xml</b></td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>7.</b></td><td>Within the MIRTH_MIGRATOR-channel click on <b>tab "Summary"</b> (1st tab) and press <b>"Set Dependencies"</b></td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>8.</b></td><td>Choose the <b>tab "Library Resources"</b> (2nd tab) in the up-popping dialog and activate the <b>checkbox</b> for <b>"Mirth Migrator"</b></td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>9.</b></td><td><b>Press ok</b>, <b>save</b> the channel changes and <b>deploy</b> the channel</td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
  <tr><td><b>10.</b></td><td>Mirth Migrator should now be available under <b>http://&lt;YOUR MIRTH SERVER&gt;:1339/MirthMigrator</b></td><td><kbd><img src="https://github.com/odoodo/Mirth-Migrator/assets/61003874/9ba37e59-896c-4fb0-897c-2f133880d82f" width="160"></kbd></td></tr>
</table>

<h2>Configuration</h2>
Mirth Migrator does not yet feature a graphical configuration frontend. (might be added at a later point of time)
Thus, the configuration has to be changed in the configuration file directly.<br/>
<br/>
This configuration file can be found at: "&lt;Your Installation Path&gt;/Mirth%20Connect/web/MirthMigrator/config/<b>MirthMigrator.conf</b>"<br/>
<br/>
The configuration consists of 4 sections:
<ul>
  <li><b>sessionLifeSpanInMinutes</b><br/>Allows to determine the maximum inactivity period for a user session in minutes. If the value is 0, the user session will not expire.</li>
<li><b>environment</b><br/>Defines the environments to which the Mirth system can be assigned. The default configuration includes the following environments:<ul><li>Production</li><li>Test</li><li>Development</li></ul>This can be changed, of course, and an arbitrary number of environments can be added.</li>
<li><b>system</b><br/></li>
<li><b>excludeFromFunctionDetection</b><br/></li>
</ul>

