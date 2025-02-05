# Profile links that will require modification / update for use with new profile pages

Desription:
The profile will be splitting contact-information and personal-information into their own respective pages, 
and therefore some links to update a specific profile item may not direct the user to the correct section. 
After looking through the vets-website codebase, we have identified 24 instances of links that go to the profile that may need
to be updated for the launch of the new profile page structure.


24 results - 20 files

```
src/applications/coronavirus-vaccination/components/Form.jsx:
  124              <a
  125:               href="/profile"
  126                target="_blank"
  
  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/disability-benefits/all-claims/content/contactInformation.jsx:
  81        of your VA accounts,{' '}
  82:       <a href="/profile">please go to your profile page.</a>
  83      </p>

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/disability-benefits/view-payments/components/view-payments-lists/ViewPaymentsLists.jsx:
  165              <p className="vads-u-margin-bottom--3">
  166:               <a href="/profile">
  167                  Go to your profile to make updates to your contact and direct
  
  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/gi/routes.jsx:
  12          <Redirect
  13:           from="/profile/:facilityCode"
  14            to="/institution/:facilityCode"
  
  - I'm not sure what this is communicating. Need to determine what is actually happening here.

src/applications/hca/enrollment-status-helpers.jsx:
  379        <p>
  380:         <a href="/profile">Go to your profile to update your address</a>.
  381        </p>
  
  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/hca/tests/components/HCAEnrollmentStatusFAQ.unit.spec.js:
  16    [HCA_ENROLLMENT_STATUSES.enrolled]:
  17: ⟪ 305 characters skipped ⟫A Form 10-10EZR</a>.</p><p>Or you can update your address and other contact information in your VA.gov profile. This will update your information across several VA benefits and services.</p><p><a href="/profile">Go to your profile to update your address</a>.</p><h3 class="vads-u-font-size--h4">Will applying again update my information?</h3><p><strong>No. A new application won’t update your information.</strong> If you have questions about the information we have on record for you, please call your nearest VA medical center.</p><p><a class="usa-button-primary" href="/find-locations/">Find your VA medical center</a></p>',
  18    [HCA_ENROLLMENT_STATUSES.ineligCHAMPVA]:

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/letters/components/NoAddressBanner.jsx:
  7        <div>
  8:         You’ll need to <a href="/profile">update your address</a> before you can
  9          view and download your VA letters or documents.
  
    - Recommendation: We could update this to /personal/contact-information, but this is not urgent since /profile redirects to /profile/personal-information, and people will still make it to the profile.

src/applications/lgy/coe/form/config/chapters/contact-information/mailing-address.js:
  13        <br />
  14:       <a href="/profile/contact-information#addresses">
  15          Update your address in your profile
  
  - Recommendation: This needs to be updated since this URL no longer exists. Should update to /profile/contact-information once the personal info revisions work goes out.
      
src/applications/my-education-benefits/config/form.js:
  421                    <p>
  422:                     <a href="/profile/personal-information">
  423                        Go to your profile

  552                    <p>
  553:                     <a href="/profile/personal-information">
  554                        Go to your profile

  652                    <p>
  653:                     <a href="/profile/personal-information">
  654                        Go to your profile

  - Recommendation: These don't need to change since /profile/personal-information is going to remain a valid URL after personal info revisions goes out.

src/applications/personalization/dashboard/components/Dashboard.jsx:
  94        <CTALink
  95:         href="/profile"
  96          text="Go to your profile"
  
  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/personalization/dashboard/components/benefit-payments-and-debts/BenefitPaymentsAndDebt.jsx:
  78              <IconCTALink
  79:               href="/profile/direct-deposit"
  80                icon="dollar-sign"
  
  - Recommendation: This doesn't need to change since /profile/direct-deposit is a valid URL
  
src/applications/personalization/profile/components/Profile.jsx:
  202                  exact
  203:                 from="/profile#contact-information"
  204                  to={PROFILE_PATHS.PERSONAL_INFORMATION}
  
  - Recommendation: This needs to be updated since this URL no longer exists. Should update to /profile/contact-information once the personal info revisions work goes out.

src/applications/personalization/profile/components/direct-deposit/PaymentInformationEditError.jsx:
  89        because your mailing address is missing or invalid. Please go back to{' '}
  90:       <a href="/profile/personal-information#edit-mailing-address">
  91          your profile

  - Recommendation: This needs to be updated since this URL will break after personal information goes out. Should update to /profile/contact-information.

src/applications/personalization/profile/tests/components/direct-deposit/PaymentInformationEditError.unit.spec.jsx:
  285      expect(wrapper.html()).to.contain(
  286:       'We’re sorry. We couldn’t update your direct deposit bank information because your mailing address is missing or invalid. Please go back to <a href="/profile/personal-information#edit-mailing-address">your profile</a> and fill in this required information.',
  287      );
  
  - Recommendation: This needs to be updated since this URL will break after personal information goes out. Should update to /profile/contact-information.
  
  297      expect(wrapper.html()).to.contain(
  298:       'We’re sorry. We couldn’t update your direct deposit bank information because your work phone number is missing or invalid. Please go back to <a href="/profile/personal-information#edit-work-phone-number">your profile</a> and fill in this required information.',
  299      );

  - Recommendation: This needs to be updated since this URL will break after personal information goes out. Should update to /profile/contact-information.

  307      expect(wrapper.html()).to.contain(
  308:       'We’re sorry. We couldn’t update your direct deposit bank information because your home phone number is missing or invalid. Please go back to <a href="/profile/personal-information#edit-home-phone-number">your profile</a> and fill in this required information.',
  309      );
  
  - Recommendation: This needs to be updated since this URL will break after personal information goes out. Should update to /profile/contact-information.

src/applications/static-pages/health-care-manage-benefits/refill-track-prescriptions-page/components/AuthContent/index.js:
  250                  <li>
  251:                   Go to your <a href="/profile/">VA.gov profile</a>.<br />
  252                    Click <strong>Edit</strong> next to each address you’d like to

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/vaos/covid-19-vaccine/components/ContactInfoPage.jsx:
  42          <br />
  43:         <NewTabAnchor href="/profile">Go to your VA profile</NewTabAnchor>.
  44        </p>

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/vaos/new-appointment/components/ContactInfoPage.jsx:
  120            <br />
  121:           <NewTabAnchor href="/profile">Go to your VA profile</NewTabAnchor>.
  122          </p>

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/vaos/new-appointment/components/CommunityCareProviderSelectionPage/ProviderSortVariant.jsx:
  132            address to{' '}
  133:           <NewTabAnchor href="/profile">your VA profile</NewTabAnchor>.
  134          </p>

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/vaos/new-appointment/components/VAFacilityPage/FacilitiesRadioWidget.jsx:
  106              address{' '}
  107:             <NewTabAnchor href="/profile">in your VA profile</NewTabAnchor>.
  108            </p>

  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information

src/applications/vre/28-1900/components/VeteranAddressDescription.jsx:
  15      </p>
  16:     <a href="/profile">
  17        Go to your profile page to update your contact information
  ```
  - Recommendation: This doesn't need to change since /profile redirects to /profile/personal-information
