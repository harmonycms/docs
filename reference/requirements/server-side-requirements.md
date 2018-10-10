# Server-side Requirements

### Operating Systems

Linux distributions \(RedHat, Ubuntu, Debian, CentOS\) are recommended for the production setup. Windows 7 and above and Mac OS X can be used for the development environment.

### Software

HarmonyCMS applications are compatible with most web servers with PHP support, but we recommend the following configuration:

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Web Server</td>
      <td style="text-align:left">
        <p><a href="https://httpd.apache.org/">Apache</a> 2.2.x or 2.4.x</p>
        <p><a href="https://www.nginx.com/">Nginx</a> (latest mainline or stable version)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">PHP</td>
      <td style="text-align:left"><a href="https://secure.php.net/">PHP</a> 7.1.3 and above</td>
    </tr>
    <tr>
      <td style="text-align:left">PHP Extensions</td>
      <td style="text-align:left">
        <ul>
          <li>openssl</li>
          <li>intl</li>
          <li>zip</li>
        </ul>
        <p></p>
      </td>
    </tr>
  </tbody>
</table>### Database

Such as Symfony, we don't provide a component to work with the database.  
However, our HarmonyFlex tool provide automatically the right Doctrine component needed to connect to the database server.

Off-course, you can install any Doctrine component to connect to your database server.

{% hint style="warning" %}
For now, only MySQL, PostgreSQL and SQLite are tested with HarmonyCMS.
{% endhint %}

