# Advanced Analytics

A repository for the group assignments.




<h3> Variables </h3>
<ul>
    <li><mark>claim_id</mark>: claim identifier (anonymized). Only used to uniquely identify each claim</li>
    <li>fraud: target (N or Y) -- was the claim fraudulent? Only available in train set</li>
    <li>claim_amount: amount paid out by the insurance company. Used to evaluate your model. Only available in train set, as this amount is not known at claim registration, i.e. early in the process.</li>
    <li>claim_date_registration: date when the claim was registered (YYYYMMDD)</li>
    <li>claim_date_occurrence: date when the accident happened (YYYYMMDD)</li>
    <li>claim_time_occurred: time when the accident happened (HHMM) -- contains many missing values</li>
    <li>claim_postal_code: location where the accident happened</li>
    <li>claim_cause: categorical variable describing what caused the accident</li>
    <li>claim_liable: whether the policy holder is to some degree liable for the accident (N or Y)</li>
    <li>claim_num_injured: number of injured parties</li>
    <li>claim_num_third_parties: number of third parties involved (e.g. in the accident)</li>
    <li>claim_num_vehicles: number of vehicles involved</li>
    <li>claim_police: whether a policy report was written up</li>
    <li>claim_alcohol: result of the alcohol test executed on the driver (Positive or Negative). A missing value indicates that no test was taken</li>
    <li>claim_language: language the claim was registered in (Dutch or French)</li>
    <li>claim_vehicle_id: the vehicle that forms the object of the claim (anonymized), i.e. the object that incurred the damage to be covered by the insurer</li>
    <li>claim_vehicle_brand: brand of the vehicle</li>
    <li>claim_vehicle_type: type of the vehicle (only cars and larger cars/vans) are considered here</li>
    <li>claim_vehicle_date_inuse: date the vehicle was registered (YYYYMM)</li>
    <li>claim_vehicle_cyl, claim_vehicle_load, claim_vehicle_fuel_type, claim_vehicle_power: additional properties describing the vehicle: cylinder contents, load capacity, fuel type and power</li>
    <li>policy_holder_id: policy holder (anonymized)</li>
    <li>policy_holder_postal_code: location of the policy holder</li>
    <li>policy_holder_form: legal form or gender of the policy holder. Only M or F in this case as we only consider retail customers</li>
    <li>policy_holder_year_birth: year of birth of the policy holder</li>
    <li>policy_holder_country: country of the policy holder (Belgium or Non-belgium)</li>
    <li>policy_holder_expert_id: identifier of the expert appointed by the policy holder to analyze the accident or damage, if any</li>
    <li>driver_id, driver_postal_code, driver_form, driver_year_birth, driver_country, driver_expert_id, driver_injured, driver_vehicle_id: similar. driver_injured indicates whether the driver was injured. Note that the driver can be different from the policy holder. vehicle_id is supposed to be the same as claim_vehicle_id, but in rarely this is not the case (most likely due to data quality issues)</li>
    <li>third_party_1_id, third_party_1_postal_code, third_party_1_injured, third_party_1_vehicle_type, third_party_1_form, third_party_1_year_birth, third_party_1_country, third_party_1_vehicle_id, third_party_1_expert_id: similar, repeated for maximally three third parties. Note that third_party_1_form can include C here (legal entity, company)</li>
    <li>repair_id, repair_postal_code, repair_form, repair_year_birth, repair_country, repair_sla: information about the repair shop which performed repairs on the damaged object. repair_sla indicates whether the repair shop has a service level agreement with the insurance company</li>
    <li>policy_date_start: date when the policy contract was started (YYYYMM)</li>
    <li>policy_date_next_expiry: next expiry date of the contract (YYYYMM)</li>
    <li>policy_date_last_renewed: date when the contract was last renewed (YYYYMM)</li>
    <li>policy_num_changes: number of changes made so far to the contract (i.e. changing the coverage, premium, etc.) so far (up until date of registration)</li>
    <li>policy_num_claims: number of previous claims registered for the contract (up until the date of registration)</li>
    <li>policy_premium_100: premium in hundreds of euros (rounded)</li>
    <li>policy_coverage_1000: coverage in thousands of euros (rounded)</li>
    <li>policy_coverage_type: included types of coverage, expressed as a binary string containing 9 bits</li>
</ul>
