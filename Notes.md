<h2>10.04.2024</h2>
<p>Since I want to use two separate databases (SQL Server for tests and a PostgreSQL for users), I am currently in a process of learning how to properly integrate both databases into EF Core.</p>
<p>Currently, I have done following:</p>
<ul>
  <li>Created an SQL Server Database for tests</li>
  <li>Added Models folder</li>
  <li>Added TestType model</li>
  <li>Added Test model</li>
  <li>Added Question model</li>
  <li>Added AnswerOption model</li>
  <li>Added tables into the Database that are corresponding to the models above (with Migration and an Update) while using code first approach</li>
</ul>
<p>Also, I have learned more about such things as DTO and Mapper so I decided to add them into a backend project as well.</p>
<p>Made a Github repository initialization and after that few pushes as well.</p>

<h2>11.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>Repository Pattern</li>
  <li>Dependency Injection</li>
  <li>Logging via Serilog</li>
  <li>How to add an SQLite database (later to be used for storing logging information.)</li>
  <li>How to implement global exception handling middleware</li>
  <li>Process of overriding ToString() method with JsonSerializer.Serialize(this)</li>
</ul>

<h2>12.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>How to make my controller action methods more maintainable through:</li>
  <ol>
    <li>Repository Pattern</li>
    <li>DTos</li>
    <li>Mapping</li>
    <li>Exception Handling</li>
    <li>Action Filters</li>
    <li>Tight Coupling</li>
  </ol>
  <li>Filters (Action Filter)</li>
  <li>ServiceFilter, TypeFilter (if arguments are required), IActionFilter</li>
</ul>

<h2>14.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>Get by id route</li>
  <li>Create route with a [FromBody] attribute</li>
  <li>Delete route</li>
  <li>HttpContent for HTTP requests</li>
  <li>CreatedAtAction</li>
  <li>Using mapper for updating an entity</li>
</ul>

<h2>15.04.2024</h2>
<p>Learned more about:</p>
<ul>
  <li>Difference between HttpPut and HttpPatch (Patch can be used for a partial update which in return can reduce a payload that is required to send. Put is used to create an entirely new object or update an already existing object fully)</li>
</ul>

<p>Did following:</p>
<ul>
  <li>Added interface for a Test repository</li>
  <li>Added repository for a Test entity</li>
  <li>Added Test controller</li>
</ul>

<p>Got introduced with an object cycle during JSON serialization.</p>
<p>Fixed it by adding a [JsonIgnore] attribute that will ignore my navigation property in a Test entity.</p>
