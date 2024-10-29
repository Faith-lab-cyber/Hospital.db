# Hospital.db
SELECT first_name, last_name, date_of_birth FROM patients;
SELECT provider_id, first_name, provider_specialty FROM providers;

SELECT * FROM patients WHERE first_name LIKE 'Ab%';
SELECT * FROM providers WHERE provider_specialty LIKE '%y';

SELECT * FROM patients WHERE date_of_birth > '1980-01-01';
SELECT * FROM visits WHERE acuity_level >= 2;

SELECT * FROM patients WHERE language = 'Spanish';
SELECT * FROM visits WHERE reason = 'Migraine' AND disposition = 'Admitted';

SELECT * FROM patients WHERE date_of_birth BETWEEN '1975-01-01' AND '1980-12-31';
SELECT first_name, last_name FROM patients ORDER BY last_name ASC;
SELECT * FROM visits ORDER BY visit_date DESC;

SELECT * FROM admissions WHERE primary_diagnosis = 'Stroke' AND discharge_disposition = 'Home';
SELECT * FROM providers WHERE join_date > '1995-01-01' AND (provider_specialty = 'Pediatrics' OR provider_specialty = 'Cardiology');

SELECT * FROM discharges WHERE discharge_disposition = 'Home' AND discharge_date BETWEEN '2018-03-01' AND '2018-03-07';


