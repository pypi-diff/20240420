# Comparing `tmp/google-contact-local-0.0.8.tar.gz` & `tmp/google-contact-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-contact-local-0.0.8.tar", last modified: Wed Jan 31 12:00:45 2024, max compression
+gzip compressed data, was "google-contact-local-0.0.9.tar", last modified: Mon Feb  5 19:51:02 2024, max compression
```

## Comparing `google-contact-local-0.0.8.tar` & `google-contact-local-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:00:45.300583 google-contact-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-31 12:00:45.300583 google-contact-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-31 11:59:42.000000 google-contact-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:00:45.300583 google-contact-local-0.0.8/google_contact_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:00:45.300583 google-contact-local-0.0.8/google_contact_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    32868 2024-01-31 11:59:42.000000 google-contact-local-0.0.8/google_contact_local/src/google_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 12:00:45.300583 google-contact-local-0.0.8/google_contact_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-31 12:00:45.000000 google-contact-local-0.0.8/google_contact_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-31 12:00:45.000000 google-contact-local-0.0.8/google_contact_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 12:00:45.000000 google-contact-local-0.0.8/google_contact_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-31 12:00:45.000000 google-contact-local-0.0.8/google_contact_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-31 12:00:45.000000 google-contact-local-0.0.8/google_contact_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-31 11:59:42.000000 google-contact-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 12:00:45.300583 google-contact-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-31 11:59:42.000000 google-contact-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 19:51:02.488573 google-contact-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-05 19:51:02.488573 google-contact-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-05 19:50:12.000000 google-contact-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 19:51:02.484573 google-contact-local-0.0.9/google_contact_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 19:51:02.484573 google-contact-local-0.0.9/google_contact_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    34258 2024-02-05 19:50:12.000000 google-contact-local-0.0.9/google_contact_local/src/google_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 19:51:02.488573 google-contact-local-0.0.9/google_contact_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-05 19:51:02.000000 google-contact-local-0.0.9/google_contact_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-05 19:51:02.000000 google-contact-local-0.0.9/google_contact_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 19:51:02.000000 google-contact-local-0.0.9/google_contact_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-05 19:51:02.000000 google-contact-local-0.0.9/google_contact_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 19:51:02.000000 google-contact-local-0.0.9/google_contact_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-05 19:50:12.000000 google-contact-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 19:51:02.488573 google-contact-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-05 19:50:12.000000 google-contact-local-0.0.9/setup.py
```

### Comparing `google-contact-local-0.0.8/README.md` & `google-contact-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `google-contact-local-0.0.8/google_contact_local/src/google_contacts.py` & `google-contact-local-0.0.9/google_contact_local/src/google_contacts.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,36 +17,38 @@
 # Local imports
 from dotenv import load_dotenv
 from location_local.locations_local_crud import LocationLocalConstants
 from user_external_local.user_externals_local import UserExternalsLocal
 from logger_local.LoggerLocal import Logger
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from user_context_remote.user_context import UserContext
-from contact_local.src.contact_local import ContactsLocal
+from contact_local.contact_local import ContactsLocal
 from database_mysql_local.generic_crud import GenericCRUD
 from contact_group_local.contact_group import ContactGroup
 from contact_notes_local.contact_notes_local import ContactNotesLocal
 from importer_local.ImportersLocal import ImportersLocal
 from contact_phones_local.contact_phones_local import ContactPhonesLocal
 from contact_profiles_local.contact_profiles_local import ContactProfilesLocal
 from contact_user_externals_local.contact_user_externals_local import ContactUserExternalsLocal
 from contact_locations_local.contact_locations_local import ContactLocationsLocal
-# from url_remote.domain import DomainLocal
+from internet_domain_local.internet_domain_local import DomainLocal
 from location_local.point import Point
 from location_local.location_local_constants import LocationLocalConstants
 from entity_type.EntityType import EntityType
 from contact_persons_local.contact_persons_local import ContactPersonsLocal
 from contact_email_address_local.contact_email_addresses_local import ContactEmailAdressesLocal
 from api_management_local.indirect import InDirect
 from api_management_local.api_limit_status import APILimitStatus
 from api_management_local.API_Mangement_Manager import APIMangementManager
 from api_management_local.Exception_API import (ApiTypeDisabledException,
                                                 ApiTypeIsNotExistException)
 from url_remote import action_name_enum, component_name_enum, entity_name_enum
 from url_remote.url_circlez import OurUrl
+from python_sdk_remote.validate_environment import validate_enviroment_variables
+# TODO: add python_sdk_remote.validate to import and call validate environment variables
 load_dotenv()
 
 # Static token details
 SCOPES = ["https://www.googleapis.com/auth/userinfo.email",
           "https://www.googleapis.com/auth/contacts.readonly",
           "openid"]  # both scopes must be allowed within the project!
 # What other scopes can we use?
@@ -67,32 +69,34 @@
 PRODUCT_USER_IDENTIFIER = os.getenv("PRODUCT_USER_IDENTIFIER")
 PRODUCT_PASSWORD = os.getenv("PRODUCT_PASSWORD")
 AUTHENTICATION_API_VERSION = 1
 
 # TODO: delete the following line when importer.insert()'s parameter location_id will have a default value
 DEFAULT_LOCATION_ID = LocationLocalConstants.UNKNOWN_LOCATION_ID
 
+
 class GoogleContacts(GenericCRUD):
     # Specific id for people api with google contacts
     GOOGLE_CONTACT_SYSTEM_ID = 6
     PEOPLE_API_ID = 16
     DATA_SOURCE_ID = 10
 
     def __init__(self, is_test_data: bool):
+        validate_enviroment_variables()
         self.user_context = UserContext.login_using_user_identification_and_password()
         # TODO: change email1, email2, email3 to email_address1, email_address2, email_address3 in ContactsLocal
         self.contacts_local = ContactsLocal(is_test_data=is_test_data)
         self.profile_id = self.user_context.get_effective_profile_id()
         self.creds = None
         self.email = None
         self.is_test_data = is_test_data
         self.client_id = os.getenv("GOOGLE_CLIENT_ID")
         self.client_secret = os.getenv("GOOGLE_CLIENT_SECRET")
 
-        # TODO Can we call a generic function in python-sdk to bring us the value and present error if there is no valye. 
+        # TODO Can we call a generic function in python-sdk to bring us the value and present error if there is no value. 
         self.port = int(os.getenv("PORT_FOR_AUTHENTICATION"))
         # Change those to consts
         self.redirect_uris = os.getenv("GOOGLE_REDIRECT_URIS")
         self.auth_uri = os.getenv("GOOGLE_AUTH_URI")
         self.token_uri = os.getenv("GOOGLE_TOKEN_URI")
         # TODO: fix https://github.com/circles-zone/entity-type-local-python-package
         # self.contact_entity_type_id = EntityType.get_entity_type_id_by_name("Contact")
@@ -195,85 +199,45 @@
         phone_numbers = [phone.get('canonicalForm') for phone in contact.get('phoneNumbers', [{}])]
         emails = [email.get('value') for email in contact.get('emailAddresses', [{}])]
         birthday = contact.get('birthdays', [{}])[0].get('text')
         location_dict = contact.get('addresses', [{}])[0]
         organizations = contact.get('organizations', [{}])[0]
         job_title = organizations.get('title')
         organization = organizations.get('name')
-        # websites = contact.get('urls', [{}])
+        websites = contact.get('urls', [{}])
         notes = contact.get('biographies')[0].get('value') if contact.get('biographies') else None
 
         # TODO: change email1, email2, email3 to email_address1, email_address2, email_address3
         # Create the dictionary
         google_contact_dict = {
             "first_name": first_name,
             "last_name": last_name,
             "display_as": display_name,
-            "phone1": phone_numbers[0] if phone_numbers else None,
             "phone_dict1": phone_dict1,
             "phone_dict2": phone_dict2,
             "phone_dict3": phone_dict3,
-            "email1": emails[0] if emails else None,
             "birthday": birthday,
             "location": location_dict,
             "job_title": job_title,
             "organization": organization,
             "notes": notes
         }
 
         # Add additional phones and emails to the dictionary
-        for i in range(1, max(len(phone_numbers), len(emails))):
+        for i in range(0, max(len(phone_numbers), len(emails), len(websites))):
             if i < len(phone_numbers):
                 google_contact_dict[f"phone{i + 1}"] = phone_numbers[i]
             if i < len(emails):
                 google_contact_dict[f"email{i + 1}"] = emails[i]
-            # if i < len(websites):
-            #     google_contact_dict[f"website{i + 1}"] = websites[i]
+            if i < len(websites):
+                google_contact_dict[f"website{i + 1}"] = websites[i].get('value')
+                google_contact_dict[f"website_type{i + 1}"] = websites[i].get('type')
+                google_contact_dict[f"website_formatted_type{i + 1}"] = websites[i].get('formattedType')
 
         return google_contact_dict
-    '''
-    @staticmethod
-    # TODO: def create_contact_object( google_contact_connection : ...) -> int
-    def create_str_representation(contact):
-
-        # TODO: our_contact Contact;
-        # Extracting relevant details from contact
-        # TODO: Extract ALL data from contact, if needed we'll add more columns in our database
-        first_names = [name.get('givenName', None) for name in contact.get('names', [])]
-        family_names = [name.get('familyName', None) for name in contact.get('names', [])]
-        phones = [phone.get('value', None) for phone in contact.get('phoneNumbers', [])]
-        emails = [email.get('value', None) for email in contact.get('emailAddresses', [])]
-        birthdays = [bday.get('text', None) for bday in contact.get('birthdays', [])]
-        addresses = [addr.get('formattedValue', None) for addr in contact.get('addresses', [])]
-        job_titles = [job.get('title', None) for job in contact.get('organizations', [])]
-        organizations = [org.get('name', None) for org in contact.get('organizations', [])]
-
-        # Create a string representation
-        str_representation = []
-        max_len = max(len(first_names), len(family_names), len(phones), len(emails), len(birthdays), len(addresses),
-                      len(job_titles), len(organizations))
-
-        for i in range(max_len):  # This part creates extra lines for multiple phone/email/etc for the same contact.
-            # Will be removed once I manage to place these values in phone1/phone2/etc rather than create an extra line.
-            first_name = first_names[i] if i < len(first_names) else first_names[-1] if first_names else None
-            family_name = family_names[i] if i < len(family_names) else family_names[-1] if family_names else None
-            phone = phones[i] if i < len(phones) else None
-            email = emails[i] if i < len(emails) else None
-            birthday = birthdays[i] if i < len(birthdays) else birthdays[-1] if birthdays else None
-            address = addresses[i] if i < len(addresses) else addresses[-1] if addresses else None
-            job_title = job_titles[i] if i < len(job_titles) else job_titles[-1] if job_titles else None
-            organization = organizations[i] if i < len(organizations) else organizations[-1] if organizations else None
-
-            # I don't think this is the right approach, we should create Contact object
-            str_representation.append(
-                f"{first_name}, {family_name}, {phone}, {birthday}, {email}, {address}, {job_title}, {organization}"
-            )
-
-        return str_representation
-    '''
 
     def pull_people_api(self, email: str):
         logger.start("Pulling Details")
         contact_id = None
         location_id = DEFAULT_LOCATION_ID
         try:
             service = build('people', 'v1', credentials=self.creds)
@@ -341,15 +305,18 @@
                         # print(arr)
                         http_status_code = http.HTTPStatus.OK.value
 
                     results = service.people().connections().list(
                         resourceName='people/me',
                         pageSize=2000,  # Scrolls further in the GoogleContacts sheet, otherwise stops at around 10 contacts.
                         pageToken=page_token,
-                        personFields='names,emailAddresses,biographies,phoneNumbers,birthdays,addresses,organizations,occupations'
+                        personFields=(
+                            'names,emailAddresses,biographies,phoneNumbers,birthdays,addresses,organizations,'
+                            'occupations,urls'
+                        )
                         ).execute()
 
                     indirct.after_call_api(external_user_id=None,
                                            api_type_id=self.PEOPLE_API_ID,
                                            endpoint=authentication_auth_login_endpoint_url, outgoing_header=headers,
                                            outgoing_body=outgoing_body,
                                            incoming_message=incoming_message,
@@ -364,92 +331,51 @@
 
                         # TODO: move these calls to ComprehensiveContacts
                         # Create dictionary representation for the contact
                         contact_dict = GoogleContacts.create_dict_representation(google_contact_connection)
 
                         # Insert or update the contact in the local database
                         contact_id = self.contacts_local.insert_update_contact(contact_dict)
-
                         try:
+                            # insert link contact_locations
+                            location_id = self._insert_link_contact_locations(contact_dict=contact_dict, contact_id=contact_id)
+                            if not location_id:
+                                location_id = DEFAULT_LOCATION_ID
+
                             # insert link contact_group
-                            contact_group = ContactGroup()
-                            contact_group.insert_contact_and_link_to_existing_or_new_group(contact_dict, contact_id,
-                                                                                           self.is_test_data)
+                            self._insert_link_contact_groups(contact_dict=contact_dict, contact_id=contact_id)
+
                             # insert link contact_persons
-                            contact_persons = ContactPersonsLocal()
-                            contact_persons.insert_contact_and_link_to_existing_or_new_person(
-                                contact_dict=contact_dict,
-                                contact_email_address=contact_dict["email1"],
-                                contact_id=contact_id
-                            )
+                            self._insert_link_contact_persons(contact_dict=contact_dict, contact_id=contact_id)
 
                             # insert link contact_email_addresses
                             self._insert_link_contact_email_addresses(contact_dict=contact_dict, contact_id=contact_id)
 
                             # insert link contact_notes
-                            contact_notes = ContactNotesLocal()
-                            contact_note_id = contact_notes.insert_contact_notes(contact_dict=contact_dict,
-                                                                                 contact_id=contact_id)
-                            contact_notes.insert_contact_note_text_block_table(contact_note_id=contact_note_id,
-                                                                               note=contact_dict["notes"])
+                            self._insert_link_contact_notes_and_text_blocks(contact_dict=contact_dict, contact_id=contact_id)
 
                             # insert link contact_phones
                             self._insert_link_contact_phones(contact_dict=contact_dict, contact_id=contact_id)
 
                             # inset link contact_user_externals
-                            contact_user_externals = ContactUserExternalsLocal()
-                            contact_user_externals.insert_contact_and_link_to_existing_or_new_user_external(
-                                contact_dict=contact_dict,
-                                contact_email_address=contact_dict["email1"],
-                                contact_id=contact_id,
-                                user_external_dict={"username": contact_dict["email1"]}
-                            )
+                            self._insert_link_contact_user_externals(contact_dict=contact_dict, contact_id=contact_id)
 
                             # insert link contact_profiles
-                            contact_profiles = ContactProfilesLocal()
-                            contact_profiles.insert_and_link_contact_profile(
-                                contact_dict=contact_dict,
-                                contact_id=contact_id
-                            )
+                            self._insert_contact_profiles(contact_dict=contact_dict, contact_id=contact_id)
 
-                            # domain_local = DomainLocal()
-                            # domain_insert_information = domain_local.link_contact_to_domain(contact_id=contact_id, url=)
-
-                            # insert link contact_locations
-                            contact_locations = ContactLocationsLocal()
-                            location_dict = self._procces_location_of_google_contact(location_dict=contact_dict["location"])
-                            contact_location_id = contact_locations.insert_contact_and_link_to_location(
-                                contact_dict=contact_dict,
-                                location_dict=location_dict,
-                                contact_id=contact_id
-                            )
-                            location_id_dict = contact_locations.select_one_dict_by_id(
-                                select_clause_value="location_id",
-                                id_column_name="contact_location_id",
-                                id_column_value=contact_location_id
-                            )
-                            location_id = location_id_dict["location_id"]
+                            # insert link contact_internet_domains
+                            self._insert_link_contact_domains(contact_dict=contact_dict, contact_id=contact_id)
 
-                            contact_locations.connection.commit()
                         except Exception as exception:
                             logger.exception(log_message="Error while inserting to contact connection tables",
                                              object={"exception": exception})
                             raise exception
                         finally:
-                            # insert link contact_importer
-                            # TODO: add correct location_id
-                            importer = ImportersLocal()
-                            user_id = self.user_context.get_effective_user_id()
-                            importer_id = importer.insert(
-                                data_source_id=self.DATA_SOURCE_ID, location_id=location_id,
-                                entity_type_id=self.contact_entity_type_id,
-                                entity_id=contact_id, url="www.google.com",
-                                user_external_id=user_external_id
-                            )
-                            logger.end()
+                            importer_id = self._insert_importer(contact_id=contact_id, location_id=location_id,
+                                                                user_external_id=user_external_id)
 
 
 
                     # TODO: Add contact_person directly or using ContactPersonsLocal.insert() from GenericCRUD
 
                     # Break after processing one contact - for debugging without running over all contacts heh
                     # break
@@ -510,14 +436,15 @@
     #     organizations = [org.get('name', None) for org in contact.get('organizations', [])]
     #     display_with_names("Organization", organizations)
 
     #     # Display occupations
     #     occupations = [occ.get('value', None) for occ in contact.get('occupations', [])]
     #     display_with_names("Occupation", occupations)
 
+
     def pull_contacts_with_stored_token(self, email):
         logger.start("Pulling Details From Existing User", object={"email": email})
         if not email:
             logger.error("Email cannot be null.")
             return
 
         logger.info("Getting token data from DB", object={"email": email, "profile_id": self.profile_id})
@@ -555,15 +482,45 @@
             logger.end()
             return
 
         # Now, pull the contacts using the People API
         self.pull_people_api(email)
         logger.end("Finished Pulling From Existing User")
 
+    def _insert_link_contact_groups(self, contact_dict: dict, contact_id: int) -> list:
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+        groups = []
+        groups_linked = None
+        if contact_dict.get("organization"):
+            groups.append(contact_dict.get("organization"))
+        if contact_dict.get("job_title"):
+            groups.append(contact_dict.get("job_title"))
+        if len(groups) > 0:
+            contact_group = ContactGroup()
+            groups_linked = contact_group.insert_contact_and_link_to_existing_or_new_group(
+                contact_dict=contact_dict,
+                contact_id=contact_id,
+                groups=groups,
+                is_test_data=self.is_test_data)
+        logger.end(object={"groups_linked": groups_linked})
+        return groups_linked
+
+    def _insert_link_contact_persons(self, contact_dict: dict, contact_id: int) -> int:
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+        contact_persons = ContactPersonsLocal()
+        contact_person_id = contact_persons.insert_contact_and_link_to_existing_or_new_person(
+            contact_dict=contact_dict,
+            contact_email_address=contact_dict["email1"],
+            contact_id=contact_id
+        )
+        logger.end(object={"contact_person_id": contact_person_id})
+        return contact_person_id
+
     def _insert_link_contact_email_addresses(self, contact_dict, contact_id):
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
         email1 = contact_dict.get("email1")
         email2 = contact_dict.get("email2")
         email3 = contact_dict.get("email3")
         contact_email_addresses = ContactEmailAdressesLocal()
         if email1:
             contact_email_addresses.insert_contact_and_link_to_email_address(
                 contact_dict=contact_dict,
@@ -578,16 +535,35 @@
             )
         if email3:
             contact_email_addresses.insert_contact_and_link_to_email_address(
                 contact_dict=contact_dict,
                 contact_email_address=email3,
                 contact_id=contact_id
             )
+        logger.end()
+
+    def _insert_link_contact_notes_and_text_blocks(self, contact_dict: dict, contact_id: int) -> int:
+        try:
+            logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+            contact_notes = ContactNotesLocal(
+                contact_dict=contact_dict,
+                contact_id=contact_id,
+                profile_id=self.profile_id
+            )
+            contact_note_id = contact_notes.insert_contact_notes()
+            contact_notes.insert_contact_note_text_block_table(contact_note_id=contact_note_id)
+            logger.end(object={"contact_note_id": contact_note_id})
+            return contact_note_id
+        except Exception as exception:
+            logger.exception(log_message="Error while inserting to contact_notes and text_blocks",
+                             object={"exception": exception})
+            return None
 
     def _insert_link_contact_phones(self, contact_dict: dict, contact_id: int):
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
         phone_dict1 = contact_dict.get("phone_dict1")
         phone1 = phone_dict1.get("canonicalForm") if phone_dict1 else None
         phone_dict2 = contact_dict.get("phone_dict2")
         phone2 = phone_dict2.get("canonicalForm") if phone_dict2 else None
         phone_dict3 = contact_dict.get("phone_dict3")
         phone3 = phone_dict3.get("canonicalForm") if phone_dict3 else None
         contact_phones = ContactPhonesLocal()
@@ -605,14 +581,83 @@
             )
         if phone3:
             contact_phones.insert_contact_and_link_to_existing_or_new_phone(
                 contact_dict=contact_dict,
                 phone_number=phone3,
                 contact_id=contact_id
             )
+        logger.end()
+
+    def _insert_link_contact_user_externals(self, contact_dict: dict, contact_id: int) -> int:
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+        contact_user_externals = ContactUserExternalsLocal()
+        contact_user_external_id = contact_user_externals.insert_contact_and_link_to_existing_or_new_user_external(
+            contact_dict=contact_dict,
+            contact_email_address=contact_dict["email1"],
+            contact_id=contact_id,
+            user_external_dict={"username": contact_dict["email1"]}
+        )
+        logger.end(object={"contact_user_external_id": contact_user_external_id})
+        return contact_user_external_id
+
+    def _insert_contact_profiles(self, contact_dict: dict, contact_id: int) -> int:
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+        contact_profiles = ContactProfilesLocal()
+        contact_profile_id = contact_profiles.insert_and_link_contact_profile(
+            contact_dict=contact_dict,
+            contact_id=contact_id
+        )
+        logger.end(object={"contact_profile_id": contact_profile_id})
+        return contact_profile_id
+
+    def _insert_link_contact_domains(self, contact_dict: dict, contact_id: int) -> list[dict]:
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+        website_count = 1
+        website_url = contact_dict.get("website" + str(website_count))
+        domain_insert_information_list = []
+        while website_url:
+            domain = DomainLocal()
+            domain_insert_information = domain.link_contact_to_domain(contact_id=contact_id,  # noqa: F841
+                                                                      url=website_url)
+            domain_insert_information_list.append(domain_insert_information)
+            website_count += 1
+            website_url = contact_dict.get("website" + str(website_count))
+        logger.end(object={"domain_insert_information_list": domain_insert_information_list})
+        return domain_insert_information_list
+
+    def _insert_link_contact_locations(self, contact_dict: dict, contact_id: int) -> int:
+        logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
+        contact_locations = ContactLocationsLocal()
+        location_dict = self._procces_location_of_google_contact(location_dict=contact_dict["location"])
+        contact_location_id = contact_locations.insert_contact_and_link_to_location(
+            contact_dict=contact_dict,
+            location_dict=location_dict,
+            contact_id=contact_id
+        )
+        location_id_dict = contact_locations.select_one_dict_by_id(
+            select_clause_value="location_id",
+            id_column_name="contact_location_id",
+            id_column_value=contact_location_id
+        )
+        location_id = location_id_dict.get("location_id")
+        logger.end(object={"contact_location_id": contact_location_id, "location_id": location_id})
+        return location_id
+
+    def _insert_importer(self, contact_id: int, location_id: int, user_external_id: int) -> int:
+        logger.start(object={"contact_id": contact_id, "location_id": location_id, "user_external_id": user_external_id})
+        importer = ImportersLocal()
+        importer_id = importer.insert(
+            data_source_id=self.DATA_SOURCE_ID, location_id=location_id,
+            entity_type_id=self.contact_entity_type_id,
+            entity_id=contact_id, url="www.google.com",
+            user_external_id=user_external_id
+        )
+        importer.connection.commit()
+        logger.end(object={"importer_id": importer_id})
+        return importer_id
 
     # TODO: see if you can improve this method
     def _procces_location_of_google_contact(self, location_dict: dict) -> dict:
         """
         Process location of google contact
         :param location_dict: location_dict
         :return: location_dict
```

