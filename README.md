# Advanced Analytics

A repository for the group assignments.




<h3> Variables </h3>

* `claim_id`: claim identifier (anonymized). Only used to uniquely identify each claim
* `fraud`: target (N or Y) -- was the claim fraudulent? Only available in train set
* `claim_amount`: amount paid out by the insurance company. Used to evaluate your model. Only available in train set, as this amount is not known at claim registration, i.e. early in the process.
* `claim_date_registration`: date when the claim was registered (YYYYMMDD)
* `claim_date_occurrence`: date when the accident happened (YYYYMMDD)
* `claim_time_occurred`: time when the accident happened (HHMM) -- contains many missing values
* `claim_postal_code`: location where the accident happened
* `claim_cause`: categorical variable describing what caused the accident
* `claim_liable`: whether the policy holder is to some degree liable for the accident (N or Y)
* `claim_num_injured`: number of injured parties
* `claim_num_third_parties`: number of third parties involved (e.g. in the accident)
* `claim_num_vehicles`: number of vehicles involved
* `claim_police`: whether a policy report was written up
* `claim_alcohol`: result of the alcohol test executed on the driver (Positive or Negative). A missing value indicates that no test was taken
* `claim_language`: language the claim was registered in (Dutch or French)
* `claim_vehicle_id`: the vehicle that forms the object of the claim (anonymized), i.e. the object that incurred the damage to be covered by the insurer
* `claim_vehicle_brand`: brand of the vehicle
* `claim_vehicle_type`: type of the vehicle (only cars and larger cars/vans) are considered here
* `claim_vehicle_date_inuse`: date the vehicle was registered (YYYYMM)
* `claim_vehicle_cyl`, `claim_vehicle_load`, `claim_vehicle_fuel_type`, `claim_vehicle_power`: additional properties describing the vehicle: cylinder contents, load capacity, fuel type and power
* `policy_holder_id`: policy holder (anonymized)
* `policy_holder_postal_code`: location of the policy holder
* `policy_holder_form`: legal form or gender of the policy holder. Only M or F in this case as we only consider retail customers
* `policy_holder_year_birth`: year of birth of the policy holder
* `policy_holder_country`: country of the policy holder (Belgium or Non-belgium)
* `policy_holder_expert_id`: identifier of the expert appointed by the policy holder to analyze the accident or damage, if any
* `driver_id`, `driver_postal_code`, `driver_form`, `driver_year_birth`, `driver_country`, `driver_expert_id`, `driver_injured`, `driver_vehicle_id`: similar. driver_injured indicates whether the driver was injured. Note that the driver can be different from the policy holder. vehicle_id is supposed to be the same as claim_vehicle_id, but in rarely this is not the case (most likely due to data quality issues)
* `third_party_1_id`, `third_party_1_postal_code`, `third_party_1_injured`, `third_party_1_vehicle_type`, `third_party_1_form`, `third_party_1_year_birth`, `third_party_1_country`, `third_party_1_vehicle_id`, `third_party_1_expert_id`: similar, repeated for maximally three third parties. Note that third_party_1_form can include C here (legal entity, company)
* `repair_id`, `repair_postal_code`, `repair_form`, `repair_year_birth`, `repair_country`, `repair_sla`: information about the repair shop which performed repairs on the damaged object. repair_sla indicates whether the repair shop has a service level agreement with the insurance company
* `policy_date_start`: date when the policy contract was started (YYYYMM)
* `policy_date_next_expiry`: next expiry date of the contract (YYYYMM)
* `policy_date_last_renewed`: date when the contract was last renewed (YYYYMM)
* `policy_num_changes`: number of changes made so far to the contract (i.e. changing the coverage, premium, etc.) so far (up until date of registration)
* `policy_num_claims`: number of previous claims registered for the contract (up until the date of registration)
* `policy_premium_100`: premium in hundreds of euros (rounded)
* `policy_coverage_1000`: coverage in thousands of euros (rounded)
* `policy_coverage_type`: included types of coverage, expressed as a binary string containing 9 bits

