<table>
  <tr>
    <th>Tables</th>
    <th>Columns</th>
    <th>Meaning</th>
  </tr>
  <tr>
    <td>areas</td>
    <td>
        <ul>id</ul>
        <ul>name</ul>
        <ul>description</ul>
    </td>
    <td>List of the UFBA's areas of knowledge</td>
  </tr>
  <tr>
    <td>course_class_offers</td>
    <td>
        <ul>id</ul>
        <ul>course_id</ul>
        <ul>discipline_class_offer_id</ul>
    </td>
    <td>Relation many-to-many between the tables courses and discipline_class_offers</td>
  </tr>
  <tr>
    <td>course_disciplines</td>
    <td>
        <ul>id</ul>
        <ul>semester</ul>
        <ul>nature</ul>
        <ul>course_id</ul>
        <ul>discipline_id</ul>
        <ul>created_at</ul>
        <ul>updated_at</ul>
    </td>
    <td>Relation many-to-many between the tables couses and disciplines</td>
  </tr>
  <tr>
    <td>courses</td>
    <td>
        <ul>id</ul>
        <ul>name</ul>
        <ul>code</ul>
        <ul>created_at</ul>
        <ul>updated_at</ul>
        <ul>curriculum</ul>
        <ul>area_id</ul>
    </td>
    <td>List of the courses offered by UFBA</td>
  </tr>
  <tr>
    <td>discipline_classes</td>
    <td>
        <ul>id</ul>
        <ul>discipline_id</ul>
        <ul>class_number</ul>
    </td>
    <td>Relation many-to-one of the table disciplines</td>
  </tr>
  <tr>
    <td>discipline_class_offers</td>
    <td>
        <ul>id</ul>
        <ul>discipline_class_id</ul>
        <ul>vacancies</ul>
    </td>
    <td>Relation many-to-one of the table discipline_classes</td>
  </tr>
  <tr>
    <td>disciplines</td>
    <td>
        <ul>id</ul>
        <ul>code</ul>
        <ul>name</ul>
        <ul>created_at</ul>
        <ul>updated_at</ul>
        <ul>curriculum</ul>
        <ul>load</ul>
    </td>
    <td>List of the disciplines offered by UFBA</td>
  </tr>
  <tr>
    <td>pre_requisites</td>
    <td>
        <ul>id</ul>
        <ul>pre_discipline_id</ul>
        <ul>post_discipline_id</ul>
        <ul>created_at</ul>
        <ul>updated_at</ul>
    </td>
    <td>List of the pre-requisites of the disciplines offered by UFBA</td>
  </tr>
  <tr>
    <td>professors</td>
    <td>
        <ul>id</ul>
        <ul>name</ul>
    </td>
    <td>List of the professors teaching at UFBA</td>
  </tr>
  <tr>
    <td>professor_schedules</td>
    <td>
        <ul>id</ul>
        <ul>schedule_id</ul>
        <ul>professor_id</ul>
    </td>
    <td>Relation many-to-many of the tables schedules and professors</td>
  </tr>
  <tr>
    <td>schedules</td>
    <td>
        <ul>id</ul>
        <ul>day</ul>
        <ul>start_hour</ul>
        <ul>start_minute</ul>
        <ul>discipline_class_id</ul>
        <ul>end_hour</ul>
        <ul>end_minute</ul>
        <ul>first_class_number</ul>
        <ul>class_count</ul>
    </td>
    <td>List of the schedules of a disciplines class</td>
  </tr>
</table>